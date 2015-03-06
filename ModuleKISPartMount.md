#### `ModuleKISPartMount`

This module allow the part to be a mount for other parts by using drag and drop on it.

Sample module configuration with the default values :
```
MODULE
{
	name = ModuleKISPartMount
	bayNodeName = top
	allowRelease = true
	allowedPartName = xxx
	allowedPartName = xxx...
	sndStorePath = KIS/Sounds/containerMount
}
```

- `bayNodeName`: Name of the attach node used to determine the position and rotation of the mounted part.
- `allowRelease`: Allow mounted part to be released from context menu or action group.
- `allowedPartName`: Part name of the part allowed on the mount. Can be repeated for multiple parts.
- `sndStorePath`: Mount sound path