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

- `shortcutKeyAction`: Define what to do when eva inventory key is pressed (1..8). Can be `drop`, `equip` or `custom`.
- `useName`: 
- `usableFromEva`: 
- `usableFromContainer`: 
- `usableFromPod`: 
- `usableFromEditor`: 
- `stackable`: 
- `volumeOverride`: 
- `moveSndPath`: 
- `equipable`:
- `equipMode`: 
- `equipSlot`: 
- `equipTrait`: 
- `equipRemoveHelmet`: 
- `equipMeshName`: 
- `equipBoneName`: 
- `equipPos`: 
- `equipDir`: 