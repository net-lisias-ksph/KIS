#### `KIS settings`

You can edit the `settings.cfg` file in the KIS folder to configure the mod.

Default settings configuration :

```
KISConfig
{
	name = KISConfig
	Global
	{
		itemDebug = false
		kerbalDefaultMass = 0.094
		breathableAtmoPressure = 0.5
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
		maxVolume = 300
		openSndPath = KIS/Sounds/inventoryOpen
		closeSndPath = KIS/Sounds/inventoryClose
	}
	EvaPickup
	{
		grabKey = g	
		attachKey = h	
		allowPartAttach = false
		allowStaticAttach = false
		allowSnapAttach = false
		maxDistance = 3
		grabMaxMass = 1
		dropSndPath = KIS/Sounds/drop
		attachPartSndPath = KIS/Sounds/attachPart
		detachPartSndPath = KIS/Sounds/detachPart
		attachStaticSndPath= KIS/Sounds/attachStatic
		detachStaticSndPath = KIS/Sounds/detachStatic
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
		moduleName = KASModuleHarpoon
		moduleName = KASModuleGrab
		moduleName = KASModuleAnchor
		moduleName = KASModuleContainer
		moduleName = USI_ModuleRecycleablePart
		moduleName = CollisionFX
	}
	StackableItemOverride
	{
		partName = addWhatYouWantHere1
		partName = addWhatYouWantHere2
	}
}
```

###### `Global`
- `itemDebug`: Enable/disable the debug tool to configure an item ingame (usefull to set position of the item on the kerbal). To use it open the context menu of an item and click "debug".
- `kerbalDefaultMass` : Set the kerbal default mass.
- `breathableAtmoPressure` : Set pressure needed to allow kerbal to remove helmet (planet with oxygen only).

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
This is the default behaviour of every kerbal for pickup. Take note that some parameters can be changed by a tool.
- `grabKey`: Shortcut key to grab
- `attachKey`: Shortcut key to attach
- `allowPartAttach`: Allow part to be attached on another part (
- `allowStaticAttach`: Allow part to be attached on static
- `allowSnapAttach`: Allow part attach with snap
- `maxDistance`: Maximum grab and move distance
- `grabMaxMass`: Maximum mass of a Kerbal can grab
- `dropSndPath`: Drop sound path
- `attachSndPath`: Attach sound path
- `attachPartSndPath`: Part ttach sound path
- `detachPartSndPath`: Part detach sound path
- `attachStaticSndPath`: Static attach sound path
- `detachStaticSndPath`: Static detach sound path
- `draggedIconResolution`: Icon resolution of the part dragged

###### `StackableModule`
- `moduleName`: Name of the stackable module. Used to determine module without any "state" saved. Part with no stackable module are set non-stackable. Part without any module are stackable by default. Can be repeated for multiple module.

###### `StackableItemOverride`
- `partName`: Name of the stackable part. Used to force a part to be stackable. Can be repeated for multiple parts.