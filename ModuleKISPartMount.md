#### `ModuleKISPartMount`

This module allow a part to be used for grabbing (all Kerbal Eva have it by default).

Sample module configuration with the default values :
```
MODULE
{
	name = ModuleKISPartMount
	bayNodeName = top
	allowRelease = true
	sndStorePath = KIS/Sounds/containerMount
}
```

- `bayNodeName`: Name of the attach node used to determine the position and rotation of the mounted part.
- `allowRelease`: Allow mounted part to be released from context menu or action group.
- `sndStorePath`: Mount sound path