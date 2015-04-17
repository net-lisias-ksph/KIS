### 1.1.0 (WIP - Not released yet)
- Added inline 2.5m container (20 000L)
- Small containers can now be carried on kerbal's back (but kerbal speed is limited on ground)
- Allow part from editor scene to be dragged to inventory (for tweaking them before storing them)
- Added stack snapping (electric screwdriver only)
- Added part snapping on mount (removed "item drag to mount" behaviour)
- Added multiple node support for PartMount module  
- Added a item module to tweak some kerbal parameters when item is equipped (for modding)
- Disabled surface attach for stack part nodes
- Disabled surface attach for part not allowing it
- Increased grab range to 3 meters in settings.cfg
- "Open inventory" context menu max distance now use the grab distance from settings.cfg
- Current attach node is now displayed on the cursor
- Removed a double when changing attach node
- Show resources, cost and mass for stored containers 
- Prevent storing a container in itself
- Prevent attaching a part on itself
- Fix a crash when trying to store a command pod from the editor
- Fix item icon not returning to default rotation 

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