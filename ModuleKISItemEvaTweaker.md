#### `ModuleKISItemEvaTweaker`

This item module tweak some kerbal parameter when the item is equipped.
For exemple, this module is used on the small container to limit the kerbal speed when carried.

Sample module configuration with the default values :
```
MODULE
{
	name = ModuleKISItemEvaTweaker
        walkSpeed = -1
        runSpeed = -1
        ladderSpeed = -1
        swimSpeed = -1
        maxJumpForce = -1
}
```

- `walkSpeed`: Change the walking speed (KSP default value is 0.8).
- `runSpeed`: Change the running speed (KSP default value is 2.2).
- `ladderSpeed`: Change the ladder climbing speed (KSP default value is 0.6).
- `swimSpeed`: Change the swimming speed (KSP default value is 0.8).
- `maxJumpForce`: Change the jumping force (KSP default value is unknown).

Setting value to -1 will ignore the change (default KSP value will be used).