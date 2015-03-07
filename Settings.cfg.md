#### `KIS configuration`

You can edit the settings.cfg file in the KIS folder to configure the mod.
Default settings configuration :

```
Global
{
	itemDebug = false
}
EvaInventory
{
	inventoryKey = tab
	rightHandKey = x
	slotsX = 2
	slotsY = 4
	slotSize = 50
	itemIconResolution = 128
	selfIconResolution = 128
	maxVolume = 0.3
	openSndPath = KIS/Sounds/inventoryOpen
	closeSndPath = KIS/Sounds/inventoryClose
}
EvaPickup
{
	grabKey = g
	canDetach = false
	maxDistance = 2
	maxMass = 1
	dropSndPath = KIS/Sounds/drop
	attachSndPath = KIS/Sounds/attach
	draggedIconResolution = 64
}
StackableModule
{
	moduleName = ModuleLight
	moduleName = ModuleDockingNode
	moduleName = ModuleAlternator
	moduleName = ModuleTestSubject
	moduleName = ModuleAerodynamicLift
	moduleName = ModuleControlSurface
	moduleName = ModuleDataTransmitter
	moduleName = ModuleLiftingSurface
	moduleName = ModuleSAS
	moduleName = ModuleTripLogger
	moduleName = KASModuleStrut
	moduleName = KASModulePort
	moduleName = KASModuleMagnet
	moduleName = KASModuleGrapplingHook
	moduleName = KASModuleGrab
	moduleName = KASModuleAnchor
}
StackableItemOverride
{
	partName = addWhatYouWantHere1
	partName = addWhatYouWantHere2
}
```

###### `Global`
- `itemDebug`: Enable/disable the debug tool to configure an item ingame (usefull to set position of the item on the kerbal). To use it open the context menu of an item and click "debug".

###### `EvaInventory`
- `inventoryKey`: Shortcut key to open the current EVA inventory.
- `rightHandKey`: Shortcut key to use the current item in the right hand.
- `slotsX`: Number of horizontal slots in the EVA inventory
- `slotsY`: Number of vertical slots in the EVA inventory
- `slotSize`: Size of the slots
- `itemIconResolution`: Resolution of the item's slot icon
- `selfIconResolution`: Resolution of the kerbal's icon
- `maxVolume`: Maximum volume of the EVA inventory
- `openSndPath`: Open sound path of the inventory
- `closeSndPath`: Close sound path of the inventory

###### `EvaPickup`
- `grabKey`: Shortcut key to grab
- `canDetach`: Ability to grab attached part
- `maxDistance`: Maximum grab and move distance
- `maxMass`: Maximum mass of a Kerbal can lift
- `dropSndPath`: Drop sound path
- `attachSndPath`: Attach sound path
- `draggedIconResolution`: Icon resolution of the part dragged

###### `StackableModule`
- `moduleName`: 

###### `StackableItemOverride`
- `partName`: 