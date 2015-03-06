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
        equipTrait = <null>
        equipRemoveHelmet = false
        equipMeshName = helmet
        equipBoneName = helmet01
        equipPos = (0, 0, 0)
        equipDir = (0, 0, 0)
}
```

- `shortcutKeyAction`: Define what to do when using eva inventory shortcuts (key 1 to 8). Can be "drop", "equip" or "custom".
- `useName`: Displayed name of the use action for the context menu of the item
- `usableFromEva`: Can be used from an eva inventory
- `usableFromContainer`: Can be used from a container inventory
- `usableFromPod`: Can be used from a pod inventory
- `usableFromEditor`: Can be used from any inventory in the editor
- `stackable`: Set if the item can be stacked
- `volumeOverride`: Set the volume of the item. Set it to 0 to let KIS calculate automatically the volume from mesh.
- `moveSndPath`: Item move sound path
- `equipable`: Set if the item can be equipped
- `equipMode`: Can be "model" or "physic". "model" will only show the item model on equip and "physic" will attach the part to the kerbal Eva (please note that this last option is pretty buggy and the part will not follow Kerbal bones correctly)
- `equipSlot`: Can be any text. Right now some name are reserved lile 'rightHand' will allow the item to be used with the [x] key.
- `equipTrait`: Restrict equip to a kerbal trait. Can be "engineer, scientist or pilot". Blank set to no restriction. Other trait name are also supported if they are added to the game.
- `equipRemoveHelmet`: If set to true helmet will be removed on equip
- `equipMeshName`: Name of the mesh used to set the equip position of the item (use item debug tool to find names)
- `equipBoneName`: Name of the bone used to set the equip position of the item (use item debug tool to find names)
- `equipPos`: Relative position of the item once equipped
- `equipDir`: Relative rotation of the item once equipped