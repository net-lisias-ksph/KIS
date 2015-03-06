#### `ModuleKISPickup`

This module allow a part to be used for grabbing. (By default on all Kerbal Eva)

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

- `maxVolume`: Maximum volume of inventory. 
- `externalAccess`: Allow inventory access by right clicking on the part from outside (from EVA)
- `internalAccess`: Allow inventory access by right clicking on the part from inside (from vessel)
- `slotsX`: Number of slot on the horizontal axis.
- `slotsY`: Number of slot on the vertical axis.
- `slotSize`: Size of the slots.
- `itemIconResolution`: Resolution of the item's slot icon.
- `selfIconResolution`: Resolution of the part's icon.
- `openSndPath`: Open sound of the inventory
- `closeSndPath`: Close sound of the inventory
- `defaultMoveSndPath`: Default move sound of items in the inventory