#### `ModuleKISPickup`

This module allow a part to be used for grabbing (all Kerbal Eva have it by default).

Sample module configuration with the default values :
```
MODULE
{
	name = ModuleKISPickup
	allowPartAttach = true
	allowStaticAttach = false
	allowPartStack = false
	maxDistance = 2
	grabMaxMass = 1
	dropSndPath = KIS/Sounds/drop
	attachPartSndPath = KIS/Sounds/attachPart
	detachPartSndPath= KIS/Sounds/detachPart
	attachStaticSndPath= KIS/Sounds/attachStatic
	detachStaticSndPath= KIS/Sounds/detachStatic
}
```

- `allowPartAttach`: Allow attach/detach of part on another part. 
- `allowStaticAttach`: Allow attach/detach of part on the ground. 
- `allowPartStack`: Allow part stack.
- `maxDistance`: Maximum range of grab.
- `grabMaxMass`: Maximum movable part mass.
- `dropSndPath`: Drop sound path.
- `attachPartSndPath `: Part attach sound path.
- `detachPartSndPath`: Part detach sound path.
- `attachStaticSndPath`: Ground attach sound path.
- `detachStaticSndPath`: Ground detach sound path.