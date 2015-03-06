KIS allow coding of any item by extending the `ModuleKISItem` class (you will need to add KIS.dll as reference first).

Take note that `ModuleKISItem` class run on the **part prefab module**. Because the part do not exist in the scene when the item is in the inventory, you will need to use KIS specific methods to keep track of the corresponding `KIS_Item` class of the inventory.

Here is an exemple class to use : 

```
    public class ModuleMyAwesomeItem : ModuleKISItem
    {
        public override void OnItemUse(KIS_Item item, KIS_Item.UseFrom useFrom)
        {
        //public 
        }

        public override void OnItemUpdate(KIS_Item item)
        {

        }

        public override void OnItemGUI(KIS_Item item)
        {

        }

        public override void OnDragToPart(KIS_Item item, Part destPart)
        {

        }

        public override void OnDragToInventory(KIS_Item item, ModuleKISInventory destInventory, int destSlot)
        {

        }

        public override void OnEquip(KIS_Item item)
        {

        }

        public override void OnUnEquip(KIS_Item item)
        {

        }
    }
```
