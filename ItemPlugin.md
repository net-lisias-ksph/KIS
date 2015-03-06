KIS allow coding of any item by extending the `ModuleKISItem` class.

```
    public class ModuleMyAwesomeItem : ModuleKISItem
    {
        public override void OnItemUse(KIS_Item item, KIS_Item.UseFrom useFrom)
        {

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
