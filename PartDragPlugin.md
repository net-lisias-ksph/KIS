KIS allow coding of item drag on part by extending the `ModuleKISPartDrag` class. 
This allow to do some custom action on drag (like the container mount).

Here is an exemple class to use : 

```
    public class ModuleMyAwesomeDragPart : ModuleKISItem
    {
        public string dragIconPath = "KIS/Textures/unknow"; //Drag icon texture when hovering the part
        public string dragText = "Unknow action"; //Text when hovering the part
        public string dragText2 = "Bla bla"; //Another line of text when hovering the part

        public override void OnItemDragged(KIS_Item draggedItem)
        {
        //Run when an item is dragged on it (from an inventory) 
        }

        public override void OnPartDragged(Part draggedPart)
        {
        //Run when a part is dragged on it (from a part in the scene)
        }
    }
```
