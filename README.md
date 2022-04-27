# SSEModdingGuide

# Skyrim Special Edition: Introduction to Modding
# Preface
This document will instruct you on setting up and modding the Steam version of Skyrim Special Edition (SSE). This document is intended for beginners, so it is vital that you read and follow all instructions carefully.

By the end of this document, you should be able to:
* Setup your copy of Skyrim to function with mods.
* Learn the functions of Mod Organizer 2 (MO2), a program designed to organize and activate mods.
* Navigate and use Nexus Mods (Nexus for short), a website that hosts mods for Skyrim.
* Download and Install mods using the aforementioned program and website.
* Build a stable Skyrim experience with essential mods.

## Requirements/Assumptions
While previous modding experience is not necessary for this document, you are expected to be knowledgeable on basic computer functions. This document will require:
* The Steam edition of SSE
* Windows 7 or higher (64-bit)
* A text editor (Notepad or Notepad++)
* [Microsoft VC++ 2015-2019](https://docs.microsoft.com/en-GB/cpp/windows/latest-supported-vc-redist?view=msvc-170) (x86 and x64)
* The latest GPU drivers
* A file archiver (7-Zip, WinRAR, etc.) 


# Preparations 
This section will teach you how to prepare SSE for modding.

Before adding any mods to your game, you will need to do the following:
1. Install SSE outside of a Windows protected folder (Program Files, Program Files (x86), etc.).
2. Setup a Nexus Account.
3. Download and install Mod Organizer 2.


## Setting up Skyrim Special Edition
You will need to ensure that your copy of SSE is outside of a Windows protected folder. Windows is very protective when you try to edit anything inside of it.

### Moving your Steam Directory
By default, your Steam directory will be placed in:

**C:\Program Files(x86)\Steam\SteamApps\Common**

To move your Steam directory:

1. In your Steam client, click **Steam** > **Settings**.

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Steam%20home%20Setting%20Highlight.png)

2. Click **Downloads** > **Steam Library Folder**.
3. Click **Add Library Folder**. You will open a Steam file explorer 
4. Navigate the explorer to a location not protected by Windows, preferably in the root directory of your hard drive.
5. Click **New Folder**.
6. Enter the name of your new folder, then click **OK**.
7. Click the **folder you created**, then click **Select**.

Your Steam games are now placed in a new location.

### Installing the Game
```
NOTE: If you have already installed and played Skyrim, skip this section.
```
1. Open Steam and go to your **Library**
2. Download and install **Skyrim Special Edition** 
3. Run SSE 
4. Exit the game once you reach the main menu. (This will generate a configuration(ini) file for SSE)

## Creating a Nexus Mods Account

Most of your mods and tools will come from Nexus Mods (Nexus), a website that hosts thousands of community made mods. You cannot download anything from the website without a Nexus account.

To create a Nexus account:
1. Navigate to the [Nexus Mods](https://www.nexusmods.com/) website.
2. Click **Register** in the top right corner of the website.
3. Follow the instructions provided by the website.

## Installing Mod Organizer 2

Mod Organizer 2 (MO2) is a program that will download and manage mod files for you. See [Introduction to Nexus Mods](https://github.com/CDimang/SSEModdingGuide/edit/main/README.md#introduction-to-nexus-mods) for more info.

1. Navigate to MO2's [page on Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/6194?tab=files).
2. Click the **Files** tab.
3. Look for **Mod Organizer 2**, then click **Manual Download**. 
4. Click **Slow Download**.
5. Navigate to the download location and double click the installer.
6. Follow the procedures provided by the installer.  

# Overview of Mod Organizer 2 (MO2)

MO2 is a program used to organize, install, and manage mods for popular games such as Fallout or The Elder Scrolls.

Rather than adding mod files to the game's directory, MO2 manages mods by separating them into an isolated folder, functioning as a virtual directory. The game will read files from MO2 rather than its own directory, tricking the game into thinking it's loading its own directory. With this isolated file system, users can enable or disable mods with a click of a button. In short, the program is designed to streamline the modding process so that users of all experience can mod their own game. 

The features available in MO2 are:

* Isolate mods from the game directory.
* Enable or Disable mods with a click of a button.
* Sort mods through numerous criteria.
* Download content from Nexus through MO2.
* Present notifications such as updates or warnings for mods.
* Swap mod configurations seamlessly.
* Add additional tools or addons for a centralized modding program.

By the end of this section, you should know:

* How to setup your game for MO2
* How each user-interface (UI) element functions
* How to apply each UI element into your modding.

## Setting Up MO2

This section will explain the virtual directory, and how to set up your game for MO2.

### Instances, a Virtual Game Directory

A **Instance** will need to be created everytime you add a game to MO2. Instances are folders where mods and configurations for your games are stored. In normal circumstances, a game will read its own directory to load the content and mods installed. However, with MO2, the program will redirect the game towards the Instance folder, making the game think that it is reading its own directory. The reason for the Instance is to keep the game's directory as clean as possible, allowing users to add or delete mods with ease. 

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Virtual.png)

### Adding your Game to MO2

The following procedures will guide you on setting up your game for MO2:

1. Open MO2
2. You will be asked to create an Instance. Click **Create a Global Instance**
3. Supported MO2 games will be displayed in a list. Select **Skyrim Special Edition**, then click **Next**. 
   If SSE does not appear like in the image below, click **Browse** and navigate to your game's executable (.exe) file.
   
   ![alt text](https://github.com/CDimang/SSE-Images/blob/main/MO2%203%20Game%20manage%20HIGHLIGHT.png)

4. Enter the name of your Instance, then click **Next**.
5. Select or create a folder to serve as the Instance folder. Click **Next**
```
TIP: For ease of access, it is recommended to create an Instance folder in the same directory as your MO2.
```
6. You will need to link your Nexus account to MO2. Click **Connect to Nexus**, your browser will be redirected to a confirmation page.

   ![alt text](https://github.com/CDimang/SSE-Images/blob/main/MO2%204%20Link%20Nexus%20Account.png)

7. Click **Authorize** on the confirmation page 

   ![alt text](https://github.com/CDimang/SSE-Images/blob/main/mo2%20nexus%20confirmation.png)

8. After you receive a confirmation that Nexus and MO2 are linked, click **Next**.  
9. A window with all the information you entered (Game choice, Instance location, Nexus account, etc.) will be displayed. After confirming that all the provided information is correct, click **Finish**.


## The Interface

The interface consists of four sections:

* Toolbar
* Installation Panel
* Executables
* Plugins

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Label%20UI%20nolog.png)

The sections below will explain the functionally of each element.

## Toolbar

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20Highlight.png)

The Toolbar is a 12-button menu that can:

* Change the functionality of MO2
* Customize the UI to the users liking
* Add additional tools or executables to MO2
* Inform the user of updates, errors, or general information.

This section will explain each button and how to use them.

### Instance Manager
![alt next](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20Instance%20Icon.png)

The Instance Manager for creating and managing Instances in MO2. This feature is required whenever you want to add or switch games in MO2. 

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20Instance%20ui.png)

The left panel lists all the Instances that you've made. Clicking an item in the list will display additional information regarding the Instance; the table below represents the information that will be displayed.

| Field |Description|   
|---|---|
|**Name**   | Name of the selected Instance. You cannot rename the Instance if it is active.  |   
| **Location**  | Location of the Instance's folder. Clicking **Explore** will direct your file explorer the displayed location. |   
| **Base Folder**  |  The directory of the Instance. |  
| **Game**  |  The title of the Instance's game.| 
| **Game Location**  |  The install location of the managed game. | 

The options to manage your Instances include:

* _Create New Instance_ - Adds another game to manage (Refer to [Adding your Game to MO2](https://github.com/CDimang/SSEModdingGuide/edit/main/README.md#adding-your-game-to-mo2) for the procedures). This will be required every time you want to manage another game with MO2.
* _Open INI_ - Opens the configuration file for the Instance. This option should be left alone.
* _Delete Instance_ - Deletes the selected Instance. A window displaying all associated files will be shown before you can remove the Instance.
* _Switch to this Instance_ - MO2 will restart and switch to the selected Instance.

### Install From Archive

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20Install%20mod%20ICON.png)

The Install From Archive button will open your file explorer to select and install downloaded mods. Only mods compressed into a ZIP file can be installed.

```
TIP: Alternatively, you can click and drag ZIP files into the MO2 window to install.
```


### Browse Mod Page

![alt text](https://github.com/CDimang/SSE-Images/blob/main/toolbar%20Nexus%20Mod%20Link%20ICON.png)

The Browse Mod Page button will direct your web browser to the managed game's section on Nexus Mods (i.e. managing a Skyrim Instance will make the button direct the web browser to the Skyrim section on Nexus Mods). 

### Refresh
![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20refresh%20ICON.png)

The Refresh button will reload MO2. Use this if any changes made to MO2 (Load order change, installed or removed mods, etc.) are not immediately reflected.

### Tools

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20Tools%20ICON.png)

The Tools button is for executing additional MO2 plugins and addons. These features expand the functionality of MO2 by providing extra options to modify your games.

The tools available by default are:

* _Bethesda Software Archive (BSA) Packer_: Creates BSA files using resources from the managed game or mods. For general modding, this plugin is not needed. 
* _Fores New Idles in Skyrim_ (FNIS): A tool that allows Skyrim to have more animations. As of 2020, this plugin has been made obsolete by [Nemesis](https://github.com/ShikyoKira/Project-New-Reign---Nemesis-Main/releases), a more up to date animation tool.
* _INI Editor_: A built-in text editor that opens the game's configuration (ini) files. This will be important for editing the appearance of your game for either performance or visual reasons. The image below is an example of viewing Skyrim's ini files.

   ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20ini%20window.png)
   
As of the making of this document, most tools are now managed by the [Executables](https://github.com/CDimang/SSEModdingGuide/blob/main/README.md#executables) feature.

### Profiles

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20Profile%20ICON.png)

Multiple mod/game configurations are managed by profiles. Much like how Instances manage multiple games, profiles will manage multiple configurations of a single game. The purpose of this feature is to allow users to playtest and experiment with numerous mod configurations. 

The following information will be unique to each profile:
* Installed mods and their status (Installed/Disabled).
   *  Mods that are enabled in one profile will be disabled in another.
   *  Mods in new profiles are disabled by default.
* Priority/Load order for installed mods and plugins.
* Configuration files (If checked in profile settings).
* Save files for managed game (If checked in profile settings).

The image below is the profile manager which allows you to create, delete, and edit your profiles. Selecting any of the profiles in the list, then clicking **Select** will swap MO2 to the selected profile, mirroring any configurations set in the selected profile. 

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20Profile%20Window.png)

The options to manage your profile include:

* _Create_ - Create a new profile. Installed mods will be disabled by default in the profile.
* _Copy_ - Copy the selected profile
* _Remove_ - Delete the selected profile. This function cannot be used on the active profile.
* _Rename_ - Change the name of an existing profile.
* _INI and Save Games setting_ - Options to make the INI and Save Game files unique to each profile. By default, Save Games is disabled and INI is enabled.

### Configuration

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20config%20ICOn.png)

The Configuration settings has 8 tabs that controls the functionality of MO2 (i.e. languages, mod color coordinations, folder directory, etc.). Use this window to tailor MO2 to your liking. 

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20config%20window.png)

The table below represents what each tab controls.

| Tab |Description|   
|---|---|
|**General**   | Options for changing the displayed language, updating MO2, and setting miscellaneous options such as centering text. |   
| **Theme**  | Color settings that highlight enabled mods based on specific conditions. For more information, see FILL |   
| **ModList**  | Additional settings for the Installation Panel such as checking for mod updates, sorting the modlist, and displaying icons based on specific conditions. |  
| **Paths**  | View and change the directories setup for MO2 | 
| **Nexus**  | Displays information for the linked Nexus Mod's account. You may also link and unlink your Nexus account from here.  | 
| **Plugins**  | Lists all games and plugins that are supported in MO2  | 
| **Workaround**  | Game settings such as forced offline mode to disable online features, or always enabling the games default files when playing. For the purpose of this guide, the Workaround tab should be ignored.  | 
| **Diagnostic**  | Settings for crash logs, a text file that is automatically generated by MO2 when your game closes due to a crash. The log will contain the mods or scripts that were running at the time of the crash, this is to help you diagnose the potential problem. This file can be accessed by opening the **Overwrite** folder at the bottom of the Installation Panel.  | 

### Executables

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20Execute%20ICON.png)

The Executables is for managing programs added to MO2. When adding a program to MO2, the added program will automatically associated itself with the managed game (i.e. modding tools that edit files will automatically direct iself to the game's directory). The addition of executables is meant to make MO2 a central hub for modding your games. These additional programs can include:

* Games 
* Tools (Editing programs such as Skyrim Special Edition Edit (SSEEdit)
* Patchers
* Virtual Folders

The figure below is an example of an Executables window on a fresh SSE Instance. The left side lists all programs added to MO2 and the right side displays information associated with the selected program such as the file location. These programs are shared between all profiles. 

![alt text](https://github.com/CDimang/SSE-Images/blob/main/toolbar%20execute%20menu.png)

The options to manage your programs is located above the list. These functions are:

* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Execute%20Add.png) _Add_ - Opens the file explorer to add a supported executable to MO2.
* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Execute%20Remove.png) _Remove_ - Remove the selected executable from MO2.
* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Execute%20move%20ex.png) _Rearrange List_ - Move the selected executable up or down the list.
* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/execute%20add%20default%20plugin.png) _Add Default Plugins_ - Adds executables based on the Instance's game (i.e. adds the Skyrim executable file if the Instance is based on Skyrim). By default the Instance will have the managed game's executables setup.

To access your executables, see Executable Menu LINK THIS LATER

The image below highlights additional settings for the executables. 

![alt text](https://github.com/CDimang/SSE-Images/blob/main/toolbar%20execute%20menu%20high.png)

These additional settings include:

* _Overwrite Steam AppID_ - Allows the game's Steam ID to be overwritten (If applicable).
* _Create Files in mod instead of overwrite_ - Files that are generated by mods will be placed into their respective mod folders instead of the Overwrite folder.
* _Force Load Libraries_ - The program will automatically execute configuration libraries (DLL files) when running the executable.
* _Use application's icon for desktop shortcut_ - Use the executable's icon when creating shortcuts
* _Hide in user interface_ - The selected executable will be hidden in MO2.

For the purpose of this guide, the aforementioned settings should be kept on their default settings.

### Endorsement

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20endorse.png)

Nexus Mods uses an endorsement system which influences how much exposure a mod will get on the website based on how many users endorse the mod. This button is only for endorsing MO2 on Nexus. 

### Notification

![alt text](https://github.com/CDimang/SSE-Images/blob/main/toolbar%20warning%20high%202.png)

The Notification icon will inform you of any potential problems in your MO2 configuration. Click the icon to open a window that will explain the problem and the potential fix for it. The image below is an example of the notification window explaining the issue. Having a notification doesn't mean that your modded game won't work, but you should try to resolve the issues as they appear.

![alt text](https://github.com/CDimang/SSE-Images/blob/main/toolbar%20warning%20desc.png)

### Update Mod Organizer

![alt text](https://github.com/CDimang/SSE-Images/blob/main/toolbar%20update%20not%20ICON.png)

If available, clicking the Update Mod Organizer button will update MO2 to the latest version.

### Help

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Toolbar%20help%20ICON.png)

The Help button is a menu that will provide additional resources to teach you about MO2. The table below represents the resources available to you. 

| Resource |Description|   
|---|---|
|**Help on UI**   | Provides a quick overview of MO2's user-interface.  |   
| **Documentation**  | Directs your web browser to MO2's website to view the documentation available for MO2|   
| **Chat on Discord**  | Provides a link to the MO2 official Discord server. Here you can communicate with developers and other users for help. |  
| **Report Issue**  | Directs the web browser to MO2's bug report forum. | 
| **Tutorial**  | Starts the built-in tutorial that will explain MO2 to you. You cannot stop the tutorial once it starts.  | 
| **About**  | Displays copyright information, list of contributers, and software used in MO2.  | 
| **About Qt**  | Copyright and general information for Qt, a C++ toolkit used to develop MO2.  | 

## Installation Panel

The Installation Panel is where all installed mods will be listed. You will be able to enable, disable, organize, and sort mods in this area. This section of the document will explain each UI element of the panel and how to use each element for your mods.

### Interface Elements

The figure below highlights the important components of the panel.

![alt text](https://github.com/CDimang/SSE-Images/blob/main/Installation%20panel%20highlight%20labels%202.png)

The highlighted components in the figure above is for the following:

* _Profile Menu_ - A dropdown menu to quickly swap profiles.
* _Mod Options_ - Modlist options that includes installing a mod, dividing the modlist by categories, and enabling or disabling mods in the list.
* _File Explorer_ - Opens your file explorer for the Instance or managed game.
* _Restore/Create Backup_ - Saves the profile's modlist to be loaded at a future date. Loading a saved modlist will overwrite your modlist. The information saved includes:
   *  All installed mods.
   *  The order of the installed mods.
   *  The status (enabled or disabled) of the mods at the time of saving.
   *  Flags and notes that were active at the time of saving. 
* _Active Mod Count_ - Displays the number of enabled mods.
* _ModList_ - Lists all installed mods. Mods listed here will display their name, conflicts, flags, category, version number, and priority number. The checkboxes to the left of the mod's name will indicate the mods status via checkmark for active or blank for disabled. More information on the list will be explained in the next section.

   ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Modlist%20mods.png)
  
* _Search Bar_ - A search filter that will update the list as you input characters.
* _Mod Filter_ - Opens a side panel with options to show or hide mods based on specified conditions. The image below is an example of using the filter with three scenarios (A, B, and C respectively). Clicking the checkboxes will cycle through **show** or **hide** mods (Indicated by a green checkmark or red dash respectively).
 
   ![alt text](https://github.com/CDimang/SSE-Images/blob/main/filter%203%20example%203%20small.png)
   
   To further elaborate on the image above:
   
   * Scenario A has the **Active Mods** filter disabled, so every mod in the list is visible.
   * Scenario B has **Active Mods** set to **Show**, so only mods that are active are visible.
   * Scenario C has **Active Mods** set to **Hide**, so mods that are active are hidden.

### Sorting the ModList

Organizing your modlist will help you keep track of your installed mods, especially if you decide to install a large quantity of mods.  

One way to sort your mods is by clicking the columns at the top of the list; your mods will be arranged based on the column selected. By default, your modlist will be sorted by Priority.  

![alt text](https://github.com/CDimang/SSE-Images/blob/main/sort%20installation.png)

The table below represents the available columns to sort by.

| Category |Description|   
|---|---|
|**Mod Name**   | Modlist is organized alphabetically. |   
|**Conflict**   | Modlist is organized based on which mods are conflicting with one another. This usually occurs when mods have files of the same name. |   
| **Flags**  | Modlist is organized based on the icons assigned to them. Notification icons will only display when specific conditions are met. For more information, see Flags LINK THIS LATER |   
| **Content**  | Modlist is organized based on the category assigned by their author. If the mod has not been assigned a category, it will be set towards the bottom of the list. See Custom Categories to learn about assigning categories to mods. |  
| **Version Number**  | Modlist is organized based on their version number and if they are up to date.| 
| **Priority**  | Modlist is organized based on their assigned priority number. This number determines the order in which mods will load when opening the managed game. For more details on Priority, see Mod Priority/Load Order. | 

You can also rearrange your modlist by clicking and dragging mods through the list. This method for organizing mods should generally be done when you want to place a mod in a specific location.

```
NOTE: You cannot click and drag mods unless your modlist is sorted by Priority.
```
#### Flags

Flags are notifications that appear when the associated mod has met a specific conditions. These flags are designed to notify you if mods are interacting with one another or meeting a criteria that should be addressed. 

The flags that are displayed include:

* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Flag%20conflict%20win.png) _Conflict Win_ - Mod is overwriting files from another mod.
* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Flag%20conflict%20lose.png) _Conflict Lose_ - Mod has its files being overwritten by another mod
* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Flag%20conflict%20win%20and%20lose.png) _Conflict Win Lose_ - Mod is overwriting another mod while being overwritten by another.
* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Flag%20invalid%20file%20mod.png) _Invalid_ - Mod contains invalid files that cannot be read by MO2. Mods associated with this flag cannot be enabled.
* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Flag%20unendorsed.png) _Unendorsed_ - Mod has not been endorsed by the user. After you install a mod, this icon will appear after an undetermined amount of time.
* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Flag%20personal%20note.png) _Note Added_ - Indicates that a note has been added to the mod. 
* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/Flag%20needs%20update.png) _Outdated_ - The mod is outdated and has an update available for download.
* ![alt text](https://github.com/CDimang/SSE-Images/blob/main/flag%20wrong.png) _Wrong Game/Version_ - Mod is for a different game.


#### Custom Categories


### ModList Color Highlights
### Mod Priority/Load Order
### Overwrite Folder


# Introduction to Nexus Mods
# Downloading and Installing Mods
# Essential Mods for Skyrim
# Closing Thoughts 
