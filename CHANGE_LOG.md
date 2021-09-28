# Kerbal Inventory System (KIS) :: Change Log

* 2016-0218: 1.2.4 (IgorZ) for KSP 1.0
	+ 1.2.4 (17 February 2016)
		- [Feature] #96: Allow move/attach a group of parts. When grab mode is selected the whole hierarchy is highlited.
		- [Feature]: New mode "Re-dock" (shortcut: "y"). Allows moving vessels docked to the station. No need to snipe the right part to deatch, the right docking port is found automatically. The port allowed for re-docking are highlighed with green color.
		- [Enhancement] Added semi-black background when showing cursor status and hint text to improve visibility in light scenes.
		- [Enhancement] Detect and fix wrong assemblies that could have created due to a bug in the KSP editor.
		- [Enhancement] Don't allow (un)equipping when dragging/moving a part.
		- [Enhancement] When stack attaching only consider nodes that don't allow collisions.
		- [Fix] #87: Correctly handle "revert flight" action, and stop adding multiple callbacks that slow down editor UI.
		- [Fix] #97: Accept names with dots when overriding part settings in config. E.g. "mumech_MJ2_AR202" is correctly tarnslated into "mumech.MJ2.AR202".
		- [Fix] Don't equip items when loading non-eva kerbal. When vessel had multiple non-engineer kerbals, and there is one with an equipped screwdriwer an error "cannot quip" was showing on load.
