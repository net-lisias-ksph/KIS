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
		breathableAtmoPressure = 0.5

		slotHotkeysEnabled = true
		slotHotkey1 = Alpha1
		slotHotkey2 = Alpha2
		slotHotkey3 = Alpha3
		slotHotkey4 = Alpha4
		slotHotkey5 = Alpha5
		slotHotkey6 = Alpha6
		slotHotkey7 = Alpha7
		slotHotkey8 = Alpha8
	}
	Editor
	{
		partGrabModifiers = None
		PodInventory
		{
			//addToAllSeats = KIS.evapropellant
			//addToTheFirstSeatOnly = KIS.electricScrewdriver
		}
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
- `itemDebug`: Enable/disable the debug tool to configure an item ingame (useful to set position of the item on the kerbal). To use it open the context menu of an item and click "debug".
- `breathableAtmoPressure` : Set pressure needed to allow kerbal to remove helmet (planet with oxygen only).
- `slotHotkeysEnabled`: Specifies if hotkeys should be handled to (de)equip item,s from the kerbal's personal inventory.
- `slotHotkeyX`: Maps a specific key as a hotkey for the inventory item (de)equip action. Kerbal's personal inventory has exactly 8 slots, and `X` in the setting name is a slot number starting from 1. You may use value `None` to skip assignment for a particular slot. By default slots' hotkeys are bound to alpha keys 1-8.

###### `Editor`
- `partGrabModifiers`: A key modifier combination to check when starting dragging items from the editor's category list panel. By default there are no modifiers, and a simple left mouse click grabs a part. Though, if you want to let KSP or other mod to handle this action you may add modifier(s) for the KIS actions. Modifiers setting is a set of three values: `AnyAlt`, `AnyShift`, and `AnyControl`. There is a special value `None` to say there must be no modifiers. The modifiers set must match *exactly*. E.g. `AnyShift, AnyAlt` setting will only work if both shift and alt keys are pressed. If there is also a control key pressed then the drag action won't trigger since the modifiers set doesn't match.
- `PodInventory`: Allows specifying items to add into pod's inventory by default. These items will be automatically added into the seat's inventory when a pod is created in the editor. The added quantity is always `1`, and each item is placed into own inventory slot. You can add up to 8 items into kerbal's personal inventory, anything above this number will be ignored.
 - `addToAllSeats`: Specifies items that will be added into every seat's inventory. Makes sense to use it to add items that are needed by every crew member. E.g. a spare EVA propellant canister.
 - `addToTheFirstSeatOnly` specifies items that should be added into the first seat's inventory only. Can be used to add items that are needed one per a craft. E.g. a screwdriver for an engineer.

 *Note*, that item names have different spelling in part's config and in KIS settings file. When part's name has an underscore (`_`) in the name it must be changed to dot (`.`). E.g. `KIS_evapropellant` is the name in the part's config, it should be `KIS.evapropellant` in the KIS settings file.

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
- `allowPartAttach`: Allow part to be attached on another part
- `allowStaticAttach`: Allow part to be attached on static
- `allowSnapAttach`: Allow part attach with snap
- `maxDistance`: Maximum distance to open a container and grab parts.
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