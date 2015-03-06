#### `ModuleKISPickup`

This module allow a part to be used for grabbing (all Kerbal Eva have it by default).

Sample module configuration with the default values :
```
MODULE
{
	name = ModuleKISPickup
	canDetach = false
	detachMaxMass = infinity
	maxDistance = 2
	maxMass = 1
	dropSndPath = KIS/Sounds/drop
	attachSndPath = KIS/Sounds/attach
	detachSndPath = KIS/Sounds/detach
}
```

- `canDetach`: Allow detachment of part attached. 
- `detachMaxMass`: Maximum mass detachable.
- `maxDistance`: Maximum range of grab.
- `maxMass`: Maximum movable part mass.
- `dropSndPath`: Drop sound path.
- `attachSndPath`: Attach sound path.
- `detachSndPath`: Detach sound path.