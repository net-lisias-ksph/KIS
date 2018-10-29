#### `ModuleKISItem`

This module will add item specific parameters to any part 

Sample module configuration (exemple) :
```
MODULE
{
        name = ModuleKISItem
        shortcutKeyAction = drop
        useName = use
        usableFromEva = false
        usableFromContainer = false
        usableFromPod = false
        usableFromEditor = false
        stackable = false
        volumeOverride = 0
        moveSndPath = KIS/Sounds/itemMove
        equipable = false
        equipMode = model
        equipSlot = <null>
        equipSkill = <null>
        equipRemoveHelmet = false
        equipBoneName = aliasHelmet
        equipPos = (0, 0, 0)
        equipDir = (0, 0, 0)
        carriable = false
        allowPartAttach = 2    
        allowStaticAttach = 0
}
```

- `shortcutKeyAction`: Define what to do when using eva inventory shortcuts (key 1 to 8). Can be "drop", "equip" or "custom" ("custom" is for plugin developers)
- `useName`: Displayed name of the use action for the context menu of the item
- `usableFromEva`: Can be used from an eva inventory
- `usableFromContainer`: Can be used from a container inventory
- `usableFromPod`: Can be used from a pod inventory
- `usableFromEditor`: Can be used from any inventory in the editor
- `stackable`: Set if the item can be stacked
- `volumeOverride`: Set the volume of the item. Set it to 0 to let KIS calculate automatically the volume from mesh.
- `moveSndPath`: Item move sound path
- `equipable`: Set if the item can be equipped
- `equipMode`: Can be "model", "part" or "physic". "model" will only show the item model on equip, "part" will spawn the part (without rigidbody however) and attach it to the kerbal (so the part modules will run normally) and "physic" will spawn and "attach" physically the part to the kerbal Eva (but it will make the eva RCS not working correctly in space and the part will not follow Kerbal bones).
- `equipSlot`: Can be any text. Right now some name are reserved like 'rightHand' will allow the item to be used with the [x] key.
- `equipSkill`: Restrict equip to a kerbal trait. Can be "engineer", "scientist" or "pilot". Leave blank set to no restriction. Other trait name are also supported if they are added to the game.
- `equipRemoveHelmet`: If set to true helmet will be removed on equip
- `equipBoneName`: Alias or search pattern to find the bone used to set the equip position of the item. Read more on the dedicated [Wiki page](https://github.com/ihsoft/KIS/wiki/Equippable-items-in-KIS-v1.15-and-higher).
- `equipPos`: Relative position of the item once equipped
- `equipDir`: Relative rotation of the item once equipped
- `carriable`: Allow the part to be carried by a kerbal. Carriable item use the 'equipSlot' parameter to check if the slot is used (it's possible to carry multiple item using different slot name).
- `allowPartAttach`: Allow the item to be attached on another part or not. 0=false,  1=true, 2=An attach tool will be needed
- `allowStaticAttach`: Allow the item to be attached on the ground or not. 0=false,  1=true, 2=An attach tool will be needed
- `staticAttachBreakForce`: Force to apply to break the ground attachement.
