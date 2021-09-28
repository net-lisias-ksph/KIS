# Kerbal Inventory System (KIS) :: Change Log

* 2016-0502: 1.2.8 (IgorZ) for KSP 1.1.2.
	+ 1.2.8 (2 May 2016)
		- [Change] Compatibility change for KSP 1.1.2.
		- [Change] When attaching a part with stack nodes by default prefer "bottom" and "top" attach nodes as they are most used ones.
		- [Change] Turn allowPartAttach and allowStaticAttach fields of KISItem into enums. Integers are still accepted but in the new parts using of enum names is encouraged.
		- [Change] Temporarily increase breaking force of equipped items by x10 (up to 50). Old settings of 5 is too weak for such applications as eva chutes. Also see bug #128.
		- [Enhancement] Show error message when "X" is pressed and no item is equipped.
		- [Enhancement] #117: Auto add common items to the seats.
		- [Fix] #116: Mass limit is not checked when grabbing from inventory.
		- [Fix] #118: Detach of static attached part results in NPE.
		- [Fix] #119: Adding an item into inventory in the editor shows KSP error in the logs.
		- [Fix] #121: In node attach mode the connection points markers get overlapped by the part's mesh.
		- [Fix] #122: For some parts attach point is wrongly detected.
		- [Fix] #124: Parts with allowPartAttach = 1 still require a tool.
* 2016-0421: 1.2.7-alpha.5 (IgorZ) for KSP 1.1 PRE-RELEASE
	+ This is a testing version only. Do not install it unless you're participating in alpha testing.
* 2016-0416: 1.2.7-alpha.4 (IgorZ) for KSP 1.1 PRE-RELEASE
	+ This is a testing version only. Do not install it unless you're participating in alpha testing.
* 2016-0414: 1.2.7-alpha.3 (IgorZ) for KSP 1.1 PRE-RELEASE
	+ This is a testing version only. Do not install it unless you're participating in alpha testing.
* 2016-0413: 1.2.7-alpha.2 (IgorZ) for KSP 1.1 PRE-RELEASE
	+ This is a testing version only. Do not install it unless you're participating in alpha testing.
* 2016-0411: 1.2.7-alpha.1 (IgorZ) for KSP 1.1 PRE-RELEASE
	+ This is a testing version only. Do not install it unless you're participating in alpha testing.
* 2016-0422: 1.2.7 (IgorZ) for KSP 1.1
	+ 1.2.7 (21 April 2016)
		- [Change] KSP 1.1 supported!
		- [Change] Increase static attach strength on ground base to prevent joint breakage.
		- [Enhancement] Add new setting in the config to specify key modifiers that
		- activate dragging in editor category list. By default it's set to `None` which
		- preserves same behavior as in 1.0.5.
		- [Enhancement] Improved search tags and descriptions in parts.
		- [Fix] Parts got replicated and attachment didn't work when surface attaching parts onto radial adapter.
		- [Fix] React on joint break on static attached items.
		- [Fix] Match rendering queue of KIS pointer to the part's highlight renderers to prevent overlapping issue.
		- [Fix] Restore highlighting of the hovered part when deselecting a hierarchy.
		- [Fix] Fix bottom attach node on ground base to make it more stable and prevent explosions on physics start.
* 2016-0408: 1.2.6 (IgorZ) for KSP 1.1
	+ 1.2.6 (7 April 2016)
	+ This version does NOT support KSP 1.1 yet! Version 1.2.7 will.
		- [Fix]: #108: Parts with no attach nodes cannot be static attached.
		- [Change]: Some cleanup to make code more compatible with pre-release of KSP 1.1.
* 2016-0222: 1.2.5 (IgorZ) for KSP 1.0
	+ 1.2.5 (22 February 2016)
		- [Feature] #101: Allow configuring EVA inventory hotkeys via a config file.
		- [Fix] #103: Part (not seat) inventory overwritten by crew inventory when transferring crew into it.
		- [Fix] #89: Portable containers revert to previous content when dropped. For now only restrict using of such inventories to not loose items. Which promotes this bug to enchancement.
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
