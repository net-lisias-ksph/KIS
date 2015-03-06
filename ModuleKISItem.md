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

- `shortcutKeyAction`: Define what to do when using eva inventory shortcuts (key 1 to 8). Can be `drop`, `equip` or `custom`.
- `useName`: Displayed name of the use action for the context menu of the item
- `usableFromEva`: Can be used from an eva inventory
- `usableFromContainer`: Can be used from a container inventory
- `usableFromPod`: Can be used from a pod inventory
- `usableFromEditor`: Can be used from any inventory in the editor
- `stackable`: Set if the item can be stacked
- `volumeOverride`: Set the volume of the item. Set it to 0 to let KIS calculate automatically the volume from mesh.
- `moveSndPath`: Item move sound path
- `equipable`: Set if the item can be equipped
- `equipMode`: 
- `equipSlot`: 
- `equipTrait`: 
- `equipRemoveHelmet`: 
- `equipMeshName`: 
- `equipBoneName`: 
- `equipPos`: 
- `equipDir`: 