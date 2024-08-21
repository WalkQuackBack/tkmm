---
title: Using Mods
---

# Using Mods

This page will guide you on how to install mods, configure options for mods, and manage mod profiles.

## Installing Mods
You can install mods from a **file archive**, a **folder**, or from **TKMM's built-in [GameBanana](https://gamebanana.com/games/7617)** tab.

### From a File Archive

> [!TIP]
> Most mods you will find will be in a file archive format, so try this method first.

#### Format 
TKMM supports installing mods from `rar`, `zip`, `7z` and `tkcl` files.

TKCL files are the most preferred mod format when using TKMM due to mod options, customizations, lower file size, and mods working on multiple versions.

#### Installation 

There are multiple methods to install a mod from a file archive:

<p>
    <img width="650" src="./images/UseMods_01_01.png">
</p>

- Drag and Drop
  - Drag a mod archive file onto the TKMM window
- Browse for file
  - **Mod > Install File** will open a window to browse for a mod archive file
  - Keyboard shortcut <kbd>Ctrl</kbd> + <kbd>I</kbd>
- Install button
  - When more than one mod is loaded, **Install** will appear under mod list
- TKCL file association
  - If your OS has TKCL files associated with TKMM you can open them to import 

### From a Folder
> [!TIP]
> Folder based mods using TKMM is only recommended during iterative development; when distributing mods you should use a file archive format.

#### Format

To install mods from a folder, it must have a format like the following:

```
[root]
  > romfs (optional)
  > exefs (optional)
```

Any other files should be added through the packaging tab.

#### Installation

- Drag and Drop
  - Drag a mod folder onto the TKMM window
- Browse for folder
  - **Mod > Install Folder** will open a window to browse for a mod folder
  - Keyboard shortcut <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>I</kbd>

### From [GameBanana](https://gamebanana.com/games/7617)

#### Finding mods
You can scroll through the home page which is sorted either by most recently updated or submitted mods.

You can also search for mods if you know their name. **Suggested Mods** is a curated selection of mods chosen by the TKMM development team.

#### Installing mods
You can install a mod by clicking on its name. You will see a list of names which correspond to files the mod has. If you see a mod with more than one file it most likely corresponds to variations/settings or updates.

When you click Yes the mod will be packaged and installed. You can always manage your mods from the homepage.

<p>
    <img width="650" src="./images/UseMods_03_02.png">
</p>

## Mod Options
Mods packaged using TKMM can have Options to allow users to customize functionality of their mods.

### Configuration

To configure options for a given mod, click on the configuration icon to the right of the mod's name in the mod list. Alternatively, with a mod selected, there will be a <kbd>Configure Options</kbd> button found underneath the mod's thumbnail.

<p>
    <img width="650" src="./images/UseMods_04_01.png">
</p>

Under the Options area, you will see each option group the mod provides. You can deselect and select options by clicking on them.

> [!NOTE]
> If a option is labeled as **Single** you can choose one or no options.
> If it is labeled as **Multiple** you can choose multiple options.
> The **Required** signifies you must choose at least one option.

<p>
    <img width="650" src="./images/UseMods_04_02.png">
</p>

## Managing Profiles

Profiles let you switch between selections of mods, sometimes referred to as mod packs. 
<p>
    <img width="650" src="./images/UseMods_05_01.png">
</p>

You can use the <kbd>+</kbd> button located next to the profile selector to add a new profile. The text field located below controls the name of the profile.

### Mod Management

To add a mod to a profile, click the <kbd>+</kbd> button next to it in the mods list.

To remove a mod from a profile, select the mod in the profile list and click on the delete button.

To uninstall a mod from TKMM, click the delete icon next to the mod in the mod list. Uninstalling a mod from TKMM removes it from all profiles and you will have to install it again to use it.

<p>
    <img width="650" src="./images/UseMods_05_02.png">
</p>

## Merging Mods

Mod merging merges your mods together to prevent conflicts and to make sure multiple mods work well together.

### Configuring Mods

You can select whether a mod is **enabled** using the checkbox next to each mod.

You can rearrange mods by dragging them to choose which ones have priority over another.

When there are mods modifying the same files, and the file types in question do not support changelogs, the mod with the higher priority will take precedence over a lower priority mod.

### Merging/Exporting

#### To **Merged Mod Output Folder**

> [!CAUTION]
> The contents of the Merged Mod Output Folder **WILL BE DELETED PERMANENTLY** upon merging. Ensure that you are using the right folder.

If your target for mods is an emulator or you want to transfer your merged mods to another device yourself, you should use this method.

Click the <kbd>Merge</kbd> button to merge your mods together to the **Merged Mod Output Folder** specified in **Settings**.

<p>
    <img width="650" src="./images/UseMods_06_01.png">
</p>

After merging you will see an alert signifying if the merge was successful. If your merge was not successful, signified by a red line on top of the alert, you can reach out to the [TKMM Discord Server](https://discord.gg/BbVXenRFVc) for support.

<p>
    <img width="650" src="./images/UseMods_06_02.png">
</p>

#### To SD Card

If your target for mods is a physical Switch, you can export to an SD Card to get your mods onto it.

You need to have a SD Card connected to your device prior to exporting. Navigate to File > Export to SD Card, and choose your SD Card from the dialog.

<p>
    <img width="650" src="./images/UseMods_07_02.png">
</p>


> [!CAUTION]
> The romfs and exefs folders in your SD Card will be **permanently deleted** from `atmosphere/contents/0100F2C0115B6000` upon exporting.
> Ensure there is nothing you wish to keep in these folders.

Click Export to finalize. Your mods will be exported to the SD card.
