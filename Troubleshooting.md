Before escalating an issue, please, try reading through this document. If none of the described issues apply to your situation, then [grab the the game's log file](#how-to-get-the-games-log-file) and make a posting on the [KIS forum] giving as much details as you can. Please, don't post just a short message like "KIS doesn't work" - nobody will be able to help you.

# KIS inventory can only have 1L of stuff

The `KIS` setup is __wrong__, it _must_ be installed exactly as described on the [KIS forum]. When the required files are not found, the described issue shows up. Below are described some frequent mistakes that people do, but this is not an exhaustive list.

## Using GitHub release

Do not download a release archive from GitHub. It's not intended for the the mod installation.  If you did it, drop all the files you have created, and follow the instructions on the forum.

This is how the right installation looks like:

![The right KIS folder content](https://raw.githubusercontent.com/ihsoft/KIS/master/WikiImages/Screenshot-TheRighContent.PNG)

## Extracting the release archive into a wrong location

There is just one _right_ location where the `KIS` files must be located. If you changed the location either intentionally or by a mistake, you've broke the mod. To verify if that's the case, find the `KIS.dll` file. It must be located _exactly_ in the path `<game root>\GameData\KIS\Plugins\KIS.dll`. If it's not there, then drop all the files and repeat the installation, but this time extract the release archive into the right location.

If you did it right, then this is how your `GameData` folder will look like:

![The right KIS folder location](https://raw.githubusercontent.com/ihsoft/KIS/master/WikiImages/Screenshot-TheRighLocation.PNG)

# Kerbals don't have "inventory" menu item when EVA

What kerbal can have is defined via `ModuleManager` mod (a.k.a. `MM`). If it's not installed, corrupted, or of a wrong version, then there will be no `KIS` specific items in the context menu.

For `KSP 1.3`, the lowest compatible version of `MM` is `2.8.0`. Even if you use `CKAN`, and it says all the versions are OK, the version still can be wrong (there were several occurrences). Go into the `GameData` folder and check the version of the mod. Update if necessary.

![ModuleManager version](https://raw.githubusercontent.com/ihsoft/KIS/master/WikiImages/Screenshot-ModuleMangerCheck.png)

# How to get the game's log file

When the problem cannot be solved via the troubleshooting steps, the only way to resolve it is analysing the log file. However, most people don't know how to get it, or get the wrong one (e.g. `output_log.txt`). When you're requested for a log, find the file named `KSP.log` which is located in the game's root:

![KSP.log location](https://raw.githubusercontent.com/ihsoft/KIS/master/WikiImages/Screenshot-KSPLogLocation.png)

By default, Windows doesn't show the files extensions, which causes troubles when locating the right file. The game's folder has two files: `KSP.exe` (the executive game file), and `KSP.log` (the log itself). When the extensions are not shown, it's really hard to find the right one. To solve it, change the view settings in the file explorer:

![Enable file extenions](https://raw.githubusercontent.com/ihsoft/KIS/master/WikiImages/Screenshot-EnableFileExtensions.png)

# Sharing the log file

The log file is usually huge. Don't even try to copy/paste it to the forum. Instead, share the file via any free (or paid) sharing service, and provide a link on the forum. There are a lot of free services in the Internet that allow sharing files, many of them don't even require registration. However, some services put a lot of ads and scripts on their pages, so avoid using such websites.

Here are just a few services that can help you sharing the file:
* __Google Drive__. If you have email on Gmail, then you have the drive. Put the file on the drive and set the sharing permissions to "everyone with the link". Then, grab the link and post it on the forum.
* [Uploadfiles.io](https://uploadfiles.io/). Just drag-n-drop or browse for the log file. The file will be persisted there for 30 days. If you didn't get help after 30 days, then it doesn't matter anyways.
* [File Convoy](https://www.fileconvoy.com/). Browse for the log file and select a reasonable retaining period (21 days max). You may skip the e-mail option.

[KIS forum]: http://forum.kerbalspaceprogram.com/index.php?/topic/149848-13-kerbal-inventory-system-kis-v150/
