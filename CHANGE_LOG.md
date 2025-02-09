# Kerbal Inventory System (KIS) :: Change Log

* 2022-0105: 1.29 (IgorZ) for KSP ['1.12.3', '1.12.2', '1.12.1', '1.12.0']
	+ 1.29 (January 4th, 2022):
		- [Enhancement] Support game's UI scale in all dialogs.
		- [Enhancement] Reduce the EVA canister dry mass to 1kg.
		- [Fix] Total mass is not ajdusted when fuel is expended from the EVA tank.
		- [Fix] Recalculate the resources mass on load to fix wrong state of the EVA tank.
		- [Fix #394] Refuel tank throws error on refuel action.
* 2021-0116: 1.28 (IgorZ) for KSP 1.11.0
	+ 1.28 (January 15th, 2021):
		- [Fix #378] Dropped parts cannot be moved or trigger physics.
		- [Fix #379] KIS functionality interferes with the stock construction mode.
		- [Fix #380] Model equippable parts cannot be carried.
		- [Fix #381] Hide UI command doesn't play well with KIS.
		- [Fix #382] Static attach doesn't verify which joint is broken.
* 2020-1224: 1.27 (IgorZ) for KSP 1.11.0
	+ 1.27 (December 23rd, 2020):
		- [Enhancement] Check for colliders when node attaching a part.
		- [Enhancement] Add KIS inventory to the stock inventory parts: SEQ-9 & SEQ-24.
		- [Enhancement] Allow the new stock modules to be stackable.
		- [Enhancement #376] The new stock ground lights won't align properly on deploy.
		- [Fix #374] Some stock science parts cannot be added into the KIS inventory.
		- [Fix #375] Make the dropped KIS parts visible to the stock inventory system.
* 2020-0719: 1.26 (IgorZ) for KSP 1.10
	+ 1.26 (July 18th, 2020):
		- [Change] Switch to `MiniAVC-V2`.
		- [Enhancement] Add a new fun part: Snacks!
		- [Enhancement] Add a new fun part: Fallen Kerbonaut. FYI, there is a real life prototype for this part.
		- [Enhancement] Add storage lockers parts. They used to be a part of the defunc SEP mod.
		- [Enhancement #360] Use fuel type from the config for the EVA fuel canister.
		- [Fix #362] Tab Key in Map View crashes the game.
		- [Fix #364] KSP 1.10: Carriable items cannot be equipped.
* 2020-0426: 1.25 (IgorZ) for KSP ['1.9.1', '1.9']
	+ 1.25 (April 25th, 2020):
		- [Change] Stop complaining about KSP minor version change.
		- [Change] Update ES-ES localization.
* 2019-1207: 1.24 (IgorZ) for KSP ['1.8.1', '1.8']
	+ 1.24 (December 6th, 2019):
		- [Change] Add a workaround for #354 to not get GUI freezed.
		- [Fix #352] Incorrect calculation of resources on the equipped items.
* 2019-1023: 1.23 (IgorZ) for KSP 1.8
	+ 1.23 (October 23rd, 2019):
		- [Change] `KSP 1.8` compatibility. __WARNING__: the mod won't work with version lower than `KSP 1.8`!
		- [Change] Replace `Editor/partGrabModifiers` setting with `Editor/editorPartGrabAction`.
		- [Enhancement] Allow dropping KIS items on the kerbal: [Dragging equipped items](https://youtu.be/udTj7_pO2hc). Thanks to [sleepyquelea](https://github.com/sleepyquelea)!
		- [Fix #339] Inflatable habitat parts have unreasonable inventories.
		- [Fix #341] AddPodInventories not called for initial crew capacity 0.
		- [Fix #348] Volumes of some parts are too high to fit the KIS containers.
* 2019-0531: 1.22 (IgorZ) for KSP 1.7.1
	+ 1.22 (May 30th, 2019):
		- [Change] "Breaking ground" DLC support.
		- [Change] Don't allow `KIS` to deploy or move the ground experiments.
		- [Change] Allow the small cargo to be carried by kerbal.
		- [Change] Disable the default remove helmet hotkey `J` as it conflicts with "Breaking ground" DLC.
		- [Enhancement] Add medium portable cargo to carry 6 experiments.
		- [Fix #333] Robotics part trigger physics when making a hover model.
		- [Fix #334] Action icons are blurred.
* 2019-0517: 1.21 (IgorZ) for KSP 1.7
	+ 1.21 (May 16th, 2019):
		- [Fix #89] Portable containers revert to previous content when dropped.
		- [Fix #328] KIS fails on every new DLC or major patch that changes kerbal models.
		- [Fix #330] KIS containers mass and volume physically realistic. __Read the issue description for details!__
* 2019-0504: 1.20 (IgorZ) for KSP 1.7
	+ 1.20 (May 3rd, 2019)):
		- [Fix #326] Text formating in PAW menu.
* 2019-0503: 1.19 (IgorZ) for KSP 1.7
	+ 1.19 (May 2nd, 2019):
		- [Change] `KSP 1.7.*` compatibility.
		- [Change] Update ES-ES localization.
		- [Change] Make `CB-1` volume physical (no override) and allow carrying it on the kerbal's back.
		- [Fix #305] Allow grab hints menu to be turned off in KIS `settings.cfg`.
		- [Fix #311] Container item launchID incorrect at vessel launch.
		- [Fix #313] Contained item's dry-mass is incorrect in tooltip.
		- [Fix #314] KIS.Container1 cannot be selected as root part.
		- [Fix #315] When the target is too far, KIS says "too heavy".
		- [Fix #317] Stock Parts not stacking in 1.6.1 with no other mods.
		- [Fix #319] Restock part volumes is wrong when a skinned mesh is used.
		- [Fix #320] Some parts refuse to get detached.
		- [Fix #321] KIS Inventory and inflatable parts.
		- [Fix #323] EVA fuel canister has infinite reserve.
		- [Fix #324] Statically attachable parts don't attach.
* 2019-0202: 1.18 (IgorZ) for KSP ['1.6.1', '1.6.0']
	+ 1.18 (February 2nd, 2019):
		- [Change] Add an optional (yet) patch file to make the legacy KIS containers physics complient. See file `kis_physical_containers.cfg.txt`.
		- [Enhancement] Add French localization.
		- [Enhancement] Improve English part descriptions.
		- [Enhancement] Add IWC-4500 "Wyvern" part.
		- [Fix #297] IMC-15K has wrong part volume.
		- [Fix #301] "volumeOverride" is not working.
		- [Fix #302] Structurel panel has wrong nodes.
		- [Fix #303] Game's crashing on the new parts.
* 2019-0129: 1.17 (IgorZ) for KSP ['1.6.1', '1.6.0']
	+ 1.17 (January 28th, 2019):
		- KSP 1.6 support. This mod's version is not compatible with the prior versions of KSP!
		- [Enhancement] Add fun English part descriptions.
		- [Enhancement] Add Portuguese (Brazil) localization.
		- [Enhancement] Improve items&parts debug ability. See `partAlignToolKey` and `itemDebug` in the settings file.
		- [Enhancement] Add new containers: `IMiC-1500`, `ImC-3K`, `IMC-22K`, and `IGC-45K`.
		- [Enhancement] Big improvement in performance. Many inventories with items in one scene could slow down the game significantly (see #287 & #288).
		- [Enhancement #281] Use the stock functionality from the KIS code and properly support custom helmets.
		- [Enhancement #289] Take into account the container size when detecting its availability.
		- [Fix #160] Cannot deatch broken solar panel.
		- [Fix #163] Implement full support of TweakScale mod.
		- [Fix #267] Review container mount mass.
		- [Fix #273] Support part's variant when dealing with KIS container items.
		- [Fix #293] Fun parts in are not equipping.
* 2018-1030: 1.16 (IgorZ) for KSP ['1.5.1', '1.5']
	+ 1.16 (October 29th, 2018):
		- [Fix #275] No preview meshes shown.
* 2018-1027: 1.15 (IgorZ) for KSP ['1.5.1', '1.5']
	+ 1.15 (October 27th, 2018):
		- [Change] KSP 1.5.* compatibility.
		- [Fix #268] Wrong size detection on the MH expansion parts. READ #273!!!
		- [Fix #269] Equip items and remove helmet actions don't work.
		- [Fix #270] Command seats must not be allowed to have inventory.
		- [Fix #271] In some languages the CCK tags are broken.
* 2018-0719: 1.14 (IgorZ) for KSP ['1.4.4', '1.4.3', '1.4.2', '1.4.1', '1.4.0']
	+ 1.14 (July 18th, 2018):
		- [Change] Migrate to KSPDev Utils 0.37.0. A stability fix.
* 2018-0708: 1.13 (IgorZ) for KSP ['1.4.3', '1.4.2', '1.4.1', '1.4.0']
	+ Do not use this release to install the mod!!!__ It's only a sources snapshot. Go to [the forum thread](https://forum.kerbalspaceprogram.com/index.php?/topic/149848-13-kerbal-inventory-system-kis-v150/) for the complete installation instructions.
	+ 1.13 (July 7th, 2018):
			- [Change] Migrate to x64 profile. The 32-bit game mode is no more supported!
			- [Change] Migrate to KSPDev Utils 0.36.0.
			- [Enhancement] Add Italian localization (IT_it).
* 2018-0507: 1.12 (IgorZ) for KSP ['1.4.3', '1.4.2', '1.4.1', '1.4.0']
	+ Do not use this release to install the mod!!!__ It's only a sources snapshot. Go to [the forum thread](https://forum.kerbalspaceprogram.com/index.php?/topic/149848-13-kerbal-inventory-system-kis-v150/) for the complete installation instructions.
	+ 1.12 (May 6th, 2018):
			- [Fix #257] Helmet doesn't remove on the female kerbal models.
			- [Change] Upgrade to KSPDev Utils v0.33.
* 2018-0327: 1.11 (IgorZ) for KSP ['1.4.2', '1.4.1', '1.4.0']
	+ Do not use this release to install the mod!!!__ It's only a sources snapshot. Go to [the forum thread](https://forum.kerbalspaceprogram.com/index.php?/topic/149848-13-kerbal-inventory-system-kis-v150/) for the complete installation instructions.
	+ 1.11 (March 26th, 2018):
			- [Fix #248] Broken inventory for the new DLC suits.
			- [Fix #252] Allow setting type of the inventory via config.
			- [Fix #253] Kerbal preview is wrong for the expansion pack suites.
			- [Fix #253] Remove helmet doesn't work on the expansion EVA suites.
* 2018-0309: 1.10 (IgorZ) for KSP 1.4.0
	+ Do not use this release to install the mod!__ It's only a sources snapshot. Go to [the forum thread](https://forum.kerbalspaceprogram.com/index.php?/topic/149848-13-kerbal-inventory-system-kis-v150/) for the complete installation instructions.
	+ 1.10 (March 8th, 2018):
			- KSP 1.4 support.
			- [Change] Update the pods in the loading screens.
			- [Enhancement] Add Espanol localization.
* 2017-1228: 1.9 (IgorZ) for KSP ['1.3.1', '1.3']
	+ Do not use this release to install the mod!__ It's only a sources snapshot. Go to [the forum thread](https://forum.kerbalspaceprogram.com/index.php?/topic/149848-13-kerbal-inventory-system-kis-v150/) for the complete installation instructions.
	+ 1.9 (December 28th, 2017):
			- [Enhancement] Add Chinese localization.
			- [Fix #235] Items equip state is not persisted.
			- [Fix #218] Exception when moving part in the editor.
* 2017-1215: 1.8 (IgorZ) for KSP ['1.3.1', '1.3']
	+ Do not use this release to install the mod!__ It's only a sources snapshot. Go to [the forum thread](https://forum.kerbalspaceprogram.com/index.php?/topic/149848-13-kerbal-inventory-system-kis-v150/) for the complete installation instructions.
	+ 1.8 (December 14th, 2017):
			- [Enhancement] Add Spanish localization.
			- [Fix #181] Match the part's menu max distance to the inventory grab distance.
			- [Fix #230] Equipped items don't destroy on kerbals pack.
			- [Fix #233] Mounted parts are improperly aligned to the target.
			- [Fix] Correct the localization string IDs that were conflicting with KAS.
* 2017-0917: 1.7 (IgorZ) for KSP 1.3
	+ Do ___not___ use this release to install the mod! It's only a sources snapshot. Go to [the forum thread](https://forum.kerbalspaceprogram.com/index.php?/topic/149848-13-kerbal-inventory-system-kis-v150/) for the complete installation instructions.
	+ 1.7 (September 17th, 2017):
			- [Fix #224] Exception when move&attach a static attach item.
			- [Fix #225] Impossible to move items between the inventories.
* 2017-0915: 1.6 (IgorZ) for KSP 1.3
	+ Do ___not___ use this release to install the mod! It's only a sources snapshot. Go to [the forum thread](https://forum.kerbalspaceprogram.com/index.php?/topic/149848-13-kerbal-inventory-system-kis-v150/) for the complete installation instructions.
	+ 1.6 (September 14th, 2017):
			- [Enhancement] Improve the attach nodes of the KIS items (including the fun parts) to reduce the physics effects on drop.
			- [Enhancement] Implement localization support.
			- [Enhancement] Full localization for the Russian language ("ru" locale).
			- [Fix #219] Inventory GUI spontaneously closes in the editor.
			- [Fix #130] Crew transfer leaves ghost pod's inventory open.
			- [Fix #220] Equipped parts trigger physics.
			- [Fix #222] The equipped screwdriver can be attached to a part.
			- [FIx #217] Align velocities on the dropped part.
			- [FIx #207] Improve docked nodes detection in ReDock mode.
* 2017-0526: 1.5.0 (IgorZ) for KSP 1.3
	+ Do _not_ use this release to install the mod! It's only a sources snapshot. Go to the forum thread for the complete installation instructions.
	+ 1.5.0 (May 25th, 2017)
			- [Change] `OnKISAction` now accepts a dictionary parameter instead of the deprecated `BaseEventData`.
			- KSP 1.3 support.
* 2017-0502: 1.4.4 (IgorZ) for KSP 1.2.2
	+ Do _not_ use this release to install the mod! It's only a sources snapshot. Go to the forum thread for the complete installation instructions.
	+ 1.4.4 (May 1st, 2017)
			- [Enhancement] Equip kerbal models on the start screen with sample KIS items. Can be adjusted/disabled via `settings.cfg`.
			- [Enhancement] Allow the Experiment Storage Unit to be carried on a kerbal's back (Wyzard256).
			- [Fix] Proper paths in the fun parts.
* 2017-0222: 1.4.3 (IgorZ) for KSP 1.2
	+ Do _not_ use this release to install the mod! It's only a sources snapshot. Go to the forum thread for the complete installation instructions.
	+ 1.4.3 (February 22nd, 2017)
		- [Fix #107] Moving a docked port causes physics effects.
		- [Fix #158] NRE when transferring crew into a pod part without KIS inventories.
		- [Fix #199] Wrong kerbal class in inventory window info when in command seat.
		- [Fix #203] Some physicsless part trigger physics effect on move&attach.
		- [Fix #206] Using of re-dock feature blocks "detach" hotkey.
		- [Enhancement #200] Set decouple momentum on Cargo Mount to zero.
		- [Enhancement #202] Make pod seat's inventory more clear.
		- [Enhancement #204] Allow stacking KIS tools.
* 2017-0128: 1.4.2 (IgorZ) for KSP 1.2
	+ Do not use this release to install the mod! It's only a sources snapshot. Go to the forum thread for the complete installation instructions.
	+ 1.4.2 (January 28th, 2017)
		- [Fix #197] Part is created on the kerbal instead of the target vessel.
* 2017-0117: 1.4.1 (IgorZ) for KSP 1.2
	+ Do not use this release to install the mod! It's only a sources snapshot. Go to the [forum thread](http://forum.kerbalspaceprogram.com/index.php?/topic/149848-12-kerbal-inventory-system-kis-v140/) for the complete installation instructions.
	+ 1.4.1 (January 16th, 2017)
		- [Fix #183] Equipped parts are not restored on scene load.
		- [Fix #186] NRE when using container in the editor.
		- [Fix #187] EVA equipped parts behave bad when sitting in the command seat.
		- [Fix #189] Handle ESC key.
		- [Fix #194] Remove helmet state is not persisted.
		- [Fix #195] Eqipped parts collide with kerbal model.
		- [Enhancement #184] Use KSP 1.2 feature to add inventories to kerbals.
		- [Enhancement #191] Add bottom attachment node to container mount.
		- [Enhancement #192] Disallow ILC-18k on container mount.
		- [Enhancement #193] Add quadrant attachment nodes to stock 2x2 panel.
* 2016-1204: 1.4.0 (IgorZ) for KSP 1.2
	+ Do not use this release to install the mod! It's only a sources snapshot. Go to the [forum thread](http://forum.kerbalspaceprogram.com/index.php?/topic/149848-12-kerbal-inventory-system-kis-v140/) for the complete installation instructions.
	+ 1.4.0 (December 4rd, 2016)
		- [Enhancement] Add default items for the first seat into a lesser slots.
		- [Fix #178] Full mass used for empty parts for purpose of removing from containers.
		- [Fix #179] Put all KIS items into a real KSP categories.
		- [Fix #180] Persist equipped state in EVA inventories.
		- [Change] ModuleManager is now a required mod.
		- [Change] CommunityCategoryKit is now a required mod.
* 2016-1124: 1.3.1 (IgorZ) for KSP 1.2
	+ 1.3.1 (November 11th, 2016)
		- [Change] Stop using KSPDev obsolete logging methods.
		- [Fix #175] EVA cnaister stopped working.
		- [Fix #129] On initial load KIS_UISoundPlayer throws errors.
		- [Fix #176] Use new KSP 1.2 categories to sort KIS parts.
		- [Fix #152] Inventory reacts to flag writing.
		- [Fix #157] MKS/OKS: NRE when adding MK-V Comm-Lab part.
		- [Fix #135] NRE detaching and reattaching part with FAR.
		- [Change] Exclude fun parts from the release.
* 2016-1012: 1.3.0 (IgorZ) for KSP 1.2
	+ KSP 1.2 support
* 2016-0622: 1.2.12 (IgorZ) for KSP 1.1.3
	+ 1.2.12 (June 21st, 2016)
		- [Fix] #109: Sandbox mode = no repairskill for non-badass kerbals.
		- [Fix] #161: KSP 1.1.3: Missing method exception.
* 2016-0611: 1.2.11 (IgorZ) for KSP 1.1.2.
	+ 1.2.11 (June 10th, 2016)
		- [Fix] #138: NRE when switching to launch.
		- [Fix] #151: NRE in editor when using Deadly Reenter mod.
		- [Fix] #154: Items in free seats's inventory are not cleared and counted to the vessel mass.
* 2016-0524: 1.2.10 (IgorZ) for KSP 1.1.2.
	+ 1.2.10 (23 May 2016)
	+ For proper part's volume calculation Module Manager is required. Though, without it the mod will still work.
		- [Fix] #117: Fix duplication of the default items on flight revert.
		- [Fix] #140: A part get created on drag in the editor.
		- [Change] Always calculate part volume from its prefab. It's now consistent but may be not optimal in some cases. E.g. deployable parts that are deployed by default (in the mesh state) will take more space than they used to be. It may result in awkward behavior of containers that were loaded prior to the update.
		- [Change] Add a ModuleManager patch to override stock drills volume since in prefab these parts are deployed and take too much space.
		- [Fix] #141: Stop directly modifying inventory part mass.
		- [Enhancement] #148: Dropped parts get weird names.
		- [Fix] #147: Some parts don't give usable drag models from prefab.
		- [Fix] #145: Carriable items show as "carried" in the inventory.
		- [Fix] #142: Settings are always read from file.
		- [Fix] #137: Volume of Drill-O-Matic calculated incorrectly.
* 2016-0503: 1.2.9 (IgorZ) for KSP 1.1.2.
	+ 1.2.9 (3 May 2016)
		- [Change] Temporarily set surface attach node as the most preferable for default. It's a workaround until #134 is fixed.
		- [Fix] #131: Kerbals can't pull items from Inventories.
		- [Fix] #133: Concrete block doesn't attach.
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
