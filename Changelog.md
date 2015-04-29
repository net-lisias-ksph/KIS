### 1.1.0 (WIP - Not released yet)
- KSP 1.0 Compatibility
- [New Part] 2.5m inline container (20 000L)
- [New Part] Ground base (similar to KAS Pylon)
- [Feature] Part snapping on stack nodes (electric screwdriver only)
- [Feature] Containers snapping on mount (removed "item drag to mount" behaviour)
- [Feature] Small containers can now be carried on kerbal's back (but kerbal speed is limited on ground)
- [Feature] Allow part from editor scene to be dragged to inventory (for tweaking them before storing them)
- [Feature] Added multiple node support for PartMount module  
- [Feature] Added TweakScale compatibility
- [Feature] Added ability to name containers
- [Feature] Added a button in the kerbal inventory to put/remove helmet
- [Feature] Added ability to set equip to "model"(default), "part" or "physic" in ModuleKISItem
- [Feature] New item module to tweak some kerbal parameters when item is equipped (for modding)
- [Feature] Current attach node is now displayed on the cursor
- [Feature] Show science data of stored items
- [Feature] Settings.cfg file is now loaded as a confignode (allow module manager to add partModules to the Stackable list)
- [Feature] Show content resources, cost, mass and science data for stored containers
- [Change] Disabled surface attach for stack part nodes
- [Change] Disabled surface attach for part not allowing it
- [Change] Increased default grab range to 3 meters
- [Change] Part cost, mass and r&d updated for KSP 1.0
- [Change] Reduced the number of slots of the small container
- [Fix] "Open inventory" context menu max distance now use the grab distance from settings.cfg
- [Fix] Disabled editor set quantity item context menu when part is not stackable
- [Fix] Fixed a crash when trying to store a command pod from the editor
- [Fix] Fixed item icon not returning to default rotation 
- [Fix] Prevent a crash if an item is added in the same slot on loading 
- [Fix] Re-arrange inventories when size is changed
- [Fix] Removed a double when changing attach node
- [Fix] Prevent storing a container in itself
- [Fix] Prevent attaching a part on itself
- [Fix] Fixed incorrect checking of volume available when stacking in the same inventory

### 1.0.2 (5 April, 2015)
- Fix wrong mass calculation for part with resources 

### 1.0.1 (31 March, 2015)
- Change volume unit from M3 to L
- Check kerbal skill instead of trait name for tools
- Added default kerbal mass parameter in settings.cfg
- Disable drag for greyed parts in the editor to prevent storing them without bought them from research in hard mode
- Add decimals to maxVolume for the inventory module tooltip
- Prevent a part to be mounted on itself
- Fix grab not working in some specific situations
- Fix crash when dragging a container from a mount to another mount
- Fix crash when attaching a docking node
- Fix container mass calculation
- Fix inventory click-through not working correctly
- Fix framerate drops while hovering inventory in flight
- Fix debug menu not working
- Fix exception thrown on first time entering VAB
- Fix exception thrown after loading
- Fix exception thrown when using release on empty mount

### 1.0.0 (14 March, 2015)
- Initial release