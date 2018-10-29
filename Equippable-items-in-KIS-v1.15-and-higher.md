# Background

In `KSP 1.5` the kerbal models were significantly changed. It broke the old KIS approach of "attaching" external items to the kerbal suite models. To have it fixed, `KIS 1.15` had a completely new approach implemented. The new approach is not compatible with the old one, so all the third-party mods need to update their part configs.

# The change

In the old approach the location of the item attachment was defined by two arguments in the `ModuleKISItem` module:

```
	equipMeshName = body01
	equipBoneName = bn_r_mid_a01
```

...where `equipMeshName` was defining the parent object in model, and `equipBoneName` was a name of the bone in the skinned mesh. Both names were searched for the exact match, which cannot work anymore after the `KSP 1.5` change.

Now, in the new approach, the item is attached to the bone _object_. This object is searched in the whole hierarchy by a pattern, so the root object here is always the suite's model root. For this reason `equipMeshName` argument is not used anymore.

The search pattern, on the other hand, is rather complicated and depends on the bone to find. Moreover, different suites have slightly different objects hierarchy, so it may be hard or even not possible to make one single pattern which will work in any case. For this reason, `KIS` now introduces a concept of _aliases_. An alias is a predefined pattern, and there can be multiple patterns for one alias. This way, the mod can attempt searching several patterns before giving up. 

E.g. here is an example from the stock config:

```
	EquipAliases
	{
		alias = aliasHelmetModel,**/model01/helmet01
		alias = aliasHelmetModel,**/model01/female01/*helmet01
	}
```

There are two different patterns for the `aliasHelmetModel` alias: on for the male models and one for the female models. Depending on which model the kerbal is wearing, one or the other pattern will match.

The item config can specify own search pattern, but in this case there can be only one. Or it can refer an alias, defined in the KIS settings file, and have multiple patterns tried. Alias names always start from prefix `alias`, this is how the mod knows if it's a search pattern or an alias.

## Search pattern syntax

In nutshell, this syntax is what `KPDev Utils` uses to deal with the model hierarchy. Full details can be found in the doc page for [`Hierarchy.FindTransformByPath`](https://ihsoft.github.io/KSPDev/Utils/html/M_KSPDev_ModelUtils_Hierarchy_FindTransformByPath_1.htm) method. It's highly unlikely that the bone searching pattern would need all the features of the pattern specification. So, here are some basic points that should cover 99% of the cases:

- The pattern is a "path" in the object hierarchy. It consists of the components, separated by symbol `/`. Each "component" is a `GameObject` in the model hierarchy.
- Use `*` as a component name to match any name.
- Add `*` at the end of the component name to perform the prefix match. E.g. `bone*` matches any name that _starts_ with `bone`.
- Add `*` at the beginning of the component name to perform the suffix match. E.g. `*bone` matches any name that _ends_ with `bone`.
- Use `**` as a component name to indicate that the following part of the pattern should be searched at any level down below the parent component. E.g. `**/a/b` will go through all the nodes starting from the parent until path `a/b` is found. If multiple paths have matched the pattern, then the shortest path will be used.

  **_Be careful with this pattern_** since in case of not matching anything it will walk thought the whole hierarchy, starting from parent. It can badly impact the performance.


## Pre-defined aliases

To not leave the third-party mods guessing which search pattern for the bone they need to specify, `KIS` defines several patterns for some widely used attach positions.

Alias | Pattern(s) | Description
----- | ---------- | -----------
aliasLeftPalm | `**/bn_l_mid_a01` | Left hand palm bone.
aliasLeftElbow | `**/bn_l_elbow_a01` | Left hand elbow bone.
aliasRightPalm | `**/bn_r_mid_a01` | Right hand palm bone.
aliasRightElbow | `**/bn_r_elbow_a01` | Right hand elbow bone.
aliasJetpack | `**/bn_jetpack01` | Jetpack bone.
aliasHelmet | `**/bn_helmet01` | Helmet bone.
aliasHead | `**/bn_upperJaw01` | Upper part of the head bone.
aliasHelmetModel | `**/model01/helmet01`<br>`**/model01/female01/*helmet01` | Helmet root _model_. It's not a bone! This alias is used to find the helmet in the "helmet on/off" action.

## Custom aliases

There is no way to specify multiple patterns in the part config. However, when necessary, it can be worked around by adding custom aliases via a `ModuleManager` patch. The stock aliases definition lives in the [KIS settings file](https://github.com/ihsoft/KIS/blob/master/settings.cfg). To add custom aliases, simple make a patch to extend the `EquipAliases` section in this file.

```
@KISConfig:AFTER[KIS]
{
	@EquipAliases
	{
		alias = aliasCustom1,**/bn_helmet01
	}
}
```

Note, that the alias name _must_ start from the `alias` prefix. The syntax of the declaration is very simple - it's a pair of values, separated by a comma: name of the alias and the search pattern.

# Transitioning from the pre-1.15 versions

Migrating the old style part configs to the `1.15` model is simple if the attach bone was "regular" - simply choose the right alias. E.g. "electrical screwdriver" part used to be defined like this:

```
	equipMeshName = body01
	equipBoneName = bn_r_mid_a01
```

and now it's:

```
	equipBoneName = aliasRightPalm
```

If there is no suitable alias found, then adding "any level match" component to the bone name usually does the trick in `KSP 1.5` (it can change in the future versions!). E.g. in the example above the path could be rewritten from `bn_r_mid_a01` to `**/bn_r_mid_a01`, and it would work just fine.