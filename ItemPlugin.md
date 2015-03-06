KIS allow coding of any item by extending the `ModuleKISItem` class (you will need to add KIS.dll as reference first).

Take note that `ModuleKISItem` class run on the **part prefab module**. Because the part do not exist in the scene when the item is in the inventory, you will need to use KIS specific methods to keep track of the corresponding `KIS_Item` class of the inventory.

Here is an exemple class to use : 

```
    public class ModuleMyAwesomeItem : ModuleKISItem
    {
        public override void OnItemUse(KIS_Item item, KIS_Item.UseFrom useFrom)
        {
        //Run when the item is used from context menu, 'x' key press or inventory shortcut key press (1 to 8)
        }

        public override void OnItemUpdate(KIS_Item item)
        {
        // Same as update(), but run for each item in the inventory
        }

        public override void OnItemGUI(KIS_Item item)
        {
        // Same as onGUI(), but run for each item in the inventory
        }

        public override void OnDragToPart(KIS_Item item, Part destPart)
        {
        // Run when the item is dragged on another part 
        }

        public override void OnDragToInventory(KIS_Item item, ModuleKISInventory destInventory, int destSlot)
        {
        // Run when the item is dragged to an inventory
        }

        public override void OnEquip(KIS_Item item)
        {
        // Run when the item is equipped        
        }

        public override void OnUnEquip(KIS_Item item)
        {
        // Run when the item is unequipped 
        }
    }
```
