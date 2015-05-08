#### `ModuleKISPartMount`

This module allow the part to be a mount for other parts by using drag and drop on it.

Sample module configuration with the default values :
```
	MODULE
	{
		name = ModuleKISPartMount
                mountedPartNode = bottom
		sndStorePath = KIS/Sounds/containerMount
		allowRelease = true
		MOUNT
		{
			attachNode = top
			allowedPartName= KIS_Container1
			allowedPartName= KIS_Container2
		}
	}
```

- `mountedPartNode` : Attach node used on the part mounted 
- `sndStorePath`: Mount sound path
- `allowRelease`: Allow mounted part to be released from context menu or action group.
- `attachNode`: Name of the attach node used on the current part to determine the position and rotation of the mounted part.
- `allowedPartName`: Part name of the part allowed on the mount. Can be repeated for multiple parts.
- MOUNT: This node can be added several times if needed, each "MOUNT" add a mounting node on the part.