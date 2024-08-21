---
title: Getting Started
---

# Getting Started

> [!IMPORTANT]
> Before starting, make sure you have downloaded .NET 8 Runtime and the appropriate version of TKMM Launcher from [Downloads](../downloads).

## Installation

Run and install the .NET 8 Runtime, if you do not have it installed already.
After verifying you have the runtime installed correctly with the right version run the TKMM Launcher executable. The following window will open.

<p>
    <img width="650" src="./images/Launcher.png" alt="tkmm launcher window">
</p>

> [!WARNING]
> If you are installing on the Steam Deck and/or cannot run as the super-user, uncheck `Create Shortcuts` to avoid needing elevated permissions.

Click <kbd>Install</kbd> to begin the installation process.

When the installation completes, click <kbd>Launch</kbd> to open TKMM.

## Setup

> [!NOTE]
> You will need to obtain a dump of the game prior to using TKMM. If you do not already have one, you can search for how to obtain it elsewhere.

When TKMM first starts, you will be asked to configure your game path. 

<p>
    <img width="650" src="./images/Settings_NoGamePath.png" alt="invalid settings page">
</p>

Click the <kbd>...</kbd> button to browse to it's location.

> [!NOTE]
> If the setting remains invalid, make sure you have a complete game dump and you are selecting the folder named `romfs` (containing `ActorSystem`, `AI`, `AISchedule`, etc.).
>
> The game dump provided must be the same version you are using on your Switch or emulator.
>
> For example, if you are playing `v1.2.1`, make sure your game dump is `v1.2.1` as well. `v1.0.0` is not a supported version by TKMM.

After following these steps, TKMM should look similar to this.

> [!NOTE]
> Even when settings are vaild you need to save for the status bar to not show the `Invalid setting` error.

<p>
    <img width="650" src="./images/Settings_WithGamePath.png">
</p>

To learn more about configuring the TKMM settings, read through the [Settings](./settings) page.

To get started using mods, check out the [Using Mods](./using-mods) page.
