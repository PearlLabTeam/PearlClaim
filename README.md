<img src="https://github.com/PearlLabTeam/PearlClaim/blob/main/images/smallers-logo.png" width=1500 height=700>

## **Spanish** User? Check out [this](https://github.com/PearlLabTeam/PearlClaim/blob/main/README_ES.md) version of the wiki

## Introduction

PearlClaim is the premier land claiming plugin for your server, offering advanced features and complete control over
your lands. With our user-friendly, advanced GUI, you can easily edit everything in-game. Despite being in beta mode, we
are dedicated to improving the plugin and making it the best it can be. Any feedback and bug reports are welcome and
will be addressed promptly. Experience the ultimate in land claiming technology and secure your lands with PearlClaim
today.

## Dependencies

The following must be installed for PearlClaim to function properly:

- [Vault.jar](https://www.spigotmc.org/resources/vault.34315/)
- An economy plugin
- A permissions plugin

Some popular permissions plugins include:

- [LuckPerms](https://luckperms.net/)
- [UltraPermissions](https://www.spigotmc.org/resources/ultra-permissions.42678/)
- [GroupManager](https://www.spigotmc.org/resources/groupmanager.38875/)

## Table of Contents

- [Commands and Permissions](https://github.com/PearlLabTeam/PearlClaim/blob/main/README.md#Commands-and-Permissions)
- [General Configurations](https://github.com/PearlLabTeam/PearlClaim/blob/main/README.md#General-Configurations)
- [Creating and Configuring Claims](https://github.com/PearlLabTeam/PearlClaim/blob/main/README.md#Creating-and-Configuring-Claims)
- [Adding Storages to Claims](https://github.com/PearlLabTeam/PearlClaim/blob/main/README.md#Adding-Storages-to-Claims)
- [Blacklist Worlds](https://github.com/PearlLabTeam/PearlClaim/blob/main/README.md#Blacklisted-Worlds)
- [Coming from Another Claim Plugin](https://github.com/PearlLabTeam/PearlClaim/blob/main/README.md#Coming-from-Another-Claim-Plugin?)
- [API Usage](https://github.com/PearlLabTeam/PearlClaim/blob/main/README.md#API-Usage)

## Note

Please note that PearlClaim is currently in beta mode and may contain some bugs. If you encounter any difficulties, we
encourage you to reach out to us on our discord server, where we will be more than happy to assist you and resolve any
issues. Thank you for your understanding and support as we continue to improve and enhance the functionality of
PearlClaim.

## Commands and Permissions

Here is a list of available commands and their respective permissions in PearlClaim:

| Command                                       | Description                                                                                                                      | Permission                 |
|-----------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|----------------------------|
| /claim                                        | Open the config menu of a claim if standing in one                                                                               | pearlclaim.use             |
| /claim sethome                                | Set the teleportation point of your claim                                                                                        | pearlclaim.sethome         |
| /claim create                                 | Create a claim from your stored claims (if any)                                                                                  | pearlclaim.create          |
| /claim config                                 | Open the config menu of a claim if standing in one                                                                               | pearlclaim.config          |
| /claim flags                                  | Open the flags GUI of the claim you're standing on                                                                               | pearlclaim.flags           |
| /claim storage                                | Open the storages that you have available in your claim                                                                          | pearlclaim.storage         |
| /claim delete                                 | Delete the claim you're standing on                                                                                              | pearlclaim.delete          |
| /claim store                                  | Pick up and store the claim you're standing on                                                                                   | pearlclaim.store           |
| /claim members < + / - > < player >           | Add or remove the given player into the claim you're standing on                                                                 | pearlclaim.modify.members  |
| /claim role < member/admin >                  | Modify the member or admin roles from the claim you're standing on                                                               | pearlclaim.modify.roles    |
| /claim linkstorage | Link your claim's storage to a block inside your claim | pearlclaim.linkstorage
| /claim unlinstorage | Unlink your claim's storage if it is linked to a block | pearlclaim.linkstorage
| /claim admin                                  | Open the Admin Configuration GUI                                                                                                 | pearlclaim.admin           |
| /claim admin giveclaim < player > < claimID > | Give the target player the claim with the provided ID                                                                            | pearlclaim.admin           |
| /claim admin import                           | Import the claims data from EpicProtections/Protection Stones (if you want us to add more plugins please let us know on discord) | pearlclaim.admin           |
| /claim admin reload                           | Reload every file and configuration and recreate files that are missing                                                          | pearlclaim.admin           |
| <br><br>                                      | |                            |
| /claims list                                  | See a list of your created claims | pearclaim.claims.list      |
| /claims tp <claim name>                       | Teleport to your claim with that name | pearlclaim.claims.teleport |

<br><br>

### Additional Permissions

| Permission | Description | Default |
|------------|-------------|---------|
| pearlclaim.admin | Permission to override and manipulate every claim | op |
| pearlcalim.flag.* | Permission to manipulate every flag | op |
| pearlclaim.flag.pvp | Permission to manipulate the flag PVP | op |
| pearlclaim.flag.hostile_spawning | Permission to manipulate the flag HOSTILE_SPAWNING | op |
| pearlclaim.flag.peaceful_spawning | Permission to manipulate the flag PEACEFUL_SPAWNING | op |
| pearlclaim.flag.crop_growth | Permission to manipulate the flag CROP_GROWTH | op |
| pearlclaim.flag.interact | Permission to manipulate the flag INTERACT | op |
| pearlclaim.flag.containers | Permission to manipulate the flag CONTAINERS | op |
| pearlclaim.flag.explosions | Permission to manipulate the flag EXPLOSIONS | op |
| pearlclaim.flag.entity_interact | Permission to manipulate the flag ENTITY_INTERACT | op |
| pearlclaim.flag.water_flow | Permission to manipulate the flag WATER_FLOW | op |
| pearlclaim.flag.lava_flow | Permission to manipulate the flag LAVA_FLOW | op |
| pearlclaim.flag.player_fly | Permission to manipulate the flag PLAYER_FLY | op |
| pearlclaim.flag.set_home | Permission to manipulate the flag SET_HOME | op |
| pearlclaim.flag.fire_spread | Permission to manipulate the flag FIRE_SPREAD | op |
| pearlclaim.flag.pve | Permission to manipulate the flag PVE | op |
| pearlclaim.role.edit | Permission to modify a role's permissions in a claim | op |
| pearlclaims.claims.changename | Permission to change your claim's display name | op |

<br><br><br>

## General Configurations

Some general configurations that are available to admins include:
<br>

### Selection Outline

The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and
straightforward process makes it quick and effortless for administrators to adjust the setting according to their
preferences.

<img src="https://i.imgur.com/PSh4yki.png" width="" height="">
<img src="https://i.imgur.com/FVUiqCh.png" width="" height="">
<img src="https://i.imgur.com/NqPukWw.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

### Default Claims toggle

The "Default Claims toggle" option provides administrators with the ability to regulate the automatic generation of
claims for new players upon joining the server. When enabled, if PearlClaim does not detect a player data file for a new
player, it will generate one and automatically add the default claims defined within the system. This function enables a
seamless and efficient claim generation process for new players.

<img src="https://i.imgur.com/jDVTBQO.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

### Language Switching

This feature provides the ability for administrators to switch between multiple languages, ensuring that the plugin
interface and related messages are displayed in the preferred language selection.

<img src="https://i.imgur.com/X6VJuIA.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

### Claim Storage toggle

This option provides administrators with the ability to control the storage access of all claims within the system. When
the storage option is set to "Disabled," it will restrict player access to all stored claims without impacting the
actual content of the stored data.

<img src="https://i.imgur.com/JYwc76w.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

### Claim Storage Require Permission

This option determines the requirement for players to have a specific permission in order to access the storage through
the graphical user interface (GUI). When set to "required," players must possess the specified permission in order to
generate the storage in the GUI. On the other hand, if set to "not required," players will be able to see the storage
button in the GUI even without the permission. However, it is important to note that this setting does not affect the
player's ability to actually access the storage's contents, which will still require the specified permission.
<img src="https://i.imgur.com/ty2frbx.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and
straightforward process makes it quick and effortless for administrators to adjust the setting according to their
preferences.
<br><br><br>

*All of these configurations can be easily modified from the plugin's settings menu, making it quick and simple for
admins to get the plugin configured exactly how they want it.*
<br><br><br>

# Creating and Configuring Claims

Creating and modifying claims has never been simpler. PearlClaim offers an in-game claim creation system for server
administrators, providing a more intuitive and user-friendly approach compared to other plugins that require manual
modification within configuration files. To create a new claim, simply navigate to the Claims Editor GUI by clicking
the "Claims Editor" button within the Admin Configuration and then select the "Create a Claim" button. When it comes to
modifying a specific claim, simply click on it to access another GUI containing a range of customization options.

### Default Claim

This option allows administrators to set the claim as default, meaning it will be added to new players' stored claims
upon joining.

<img src="https://i.imgur.com/iUWQZlT.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

### Modify Storage

This option opens a separate GUI that enables the modification of the claim's storage settings. Additional information
can be found in the "Creating and Configuring Claims" section.

<img src="https://i.imgur.com/IKpKddo.png" width="" height="">

***Claim's Storage Editor***

<img src="https://i.imgur.com/C5VyhJe.png" width="" height="">
<br><br><br>

### Give to Player

Allows administrators to transfer the claim to another player by specifying the player's name in chat. It is important
to note that any updates made to the claim after it has been transferred will not be reflected in the recipient player's
stored claims.

<img src="https://i.imgur.com/EXw16Fz.png" width="" height=""><br><br>
<img src="https://i.imgur.com/yqd4CZD.png" width="" height=""><br><br>
<img src="https://i.imgur.com/naRxnMh.png" width="" height=""><br><br>
<img src="https://i.imgur.com/djGdTBi.png" width="" height="">
<br><br><br>

### Change Radius

Enables the adjustment of the X, Y, and Z starting radius of the claim.

<img src="https://i.imgur.com/GNyQtRi.png" width="" height=""><br><br>
<img src="https://i.imgur.com/4Lp6BiV.png" width="" height=""><br><br>
<img src="https://i.imgur.com/Wqwc9aN.png" width="" height=""><br><br>
<img src="https://i.imgur.com/GlkIqsj.png" width="" height="">
<br><br><br>

### Allow Upgrade

This option determines whether players with the claim can upgrade it using in-game currency.

<img src="https://i.imgur.com/zXPvm0H.png" width="" height=""><br><br>
If set to **UPGRADABLE,** you will need to provide values for per-block-upgrade-cost and max-upgrade-radius for all X,Y,
and Z

<img src="https://i.imgur.com/iDlBA46.png" width="" height=""><br><br>
<img src="https://i.imgur.com/FiEz2wz.png" width="" height=""><br><br>

### Creation Prompt Block

Specifies the animation block that will accompany the player when selecting land to claim. This block will indicate the
center point of the claim.

<img src="https://i.imgur.com/8nup5YJ.png" width="" height=""><br><br>
***When activated, this button will initiate the opening of a new graphical user interface with multiple pages. Within
this interface, the user will have the ability to select the material of the animation item.***

<img src="https://i.imgur.com/WpP8qtD.png" width="" height=""><br>

### Delete

Deletes the claim and all its configurations.

<img src="https://i.imgur.com/PqwY4Ub.png" width="" height=""><br>

### Back

Returns to the main menu.

<img src="https://i.imgur.com/WxAbeBL.png" width="" height=""><br>
<br><br>

# Adding Storages to Claims

We are pleased to introduce our state-of-the-art storage system for your land. Our system offers a convenient and efficient solution for virtual storage without the need for physical chests.

With a few simple clicks, you can customize every aspect of your claim's storage, including the number of storages, their size, and even premade content for a kit if desired. Our system creates a virtual storage system that is copied over to the player's claim, giving them full control over their storage needs.

**For a tutorial on how to modify the look of the storage's GUI for certain claims, watch this video** [![Tutorial](https://img.youtube.com/vi/Yr6ab1ZcWTA/0.jpg)](https://www.youtube.com/watch?v=Yr6ab1ZcWTA)

We are confident that our advanced storage system will exceed your expectations and provide you with the best possible experience. Thank you for considering our product.
<br><br>

### To begin, simply click on the "Create a Storage" button located on the Anvil.

<img src="https://i.imgur.com/xDaU8Sf.png" width="" height=""><br>

### After clicking the button, you will be prompted to enter the name of the storage, which will serve as the identifier for linking the storage to the StorageGUI file.

<img src="https://i.imgur.com/15IHfvi.png" width="" height=""><br>

### Upon providing the name, you will be required to specify the size of the storage in terms of the number of slots available in the inventory.

<img src="https://i.imgur.com/QZ0LBx1.png" width="" height=""><br>

### Once the necessary information has been entered, a new storage button will be generated within the Storage Editor GUI. If you would like to include pre-made items in the storage, simply place them inside the storage, and they will be added to the player's storage upon receipt of the claim. If you prefer an empty storage, simply omit this step.

<img src="https://i.imgur.com/crMKUWh.png" width="" height=""><br>
<img src="https://i.imgur.com/QFI4sVI.png" width="" height=""><br><br><br>

# Linking Storages to a Block

### It is very simple to connect your storage to a block to avoid typing in the storage command everytime you want to use the storage gui. Simply type in /claim linkstorage or unlinkstorage to unlink.

**For a tutorial on how this is done, look here** [![Tutorial](https://img.youtube.com/vi/Yr6ab1ZcWTA/0.jpg)](https://www.youtube.com/watch?v=zxfC2yx8YKo&t=2s)

# Blacklisted Worlds
**We understand the need to control and manage claim creation in certain regions. That is why we are proud to offer our Blacklisted Worlds system, which allows you to disable the creation of claims in designated worlds.**

**To utilize this system, simply navigate to the Blacklisted Worlds button within the Admin Configuration GUI and select the world in which you wish to block claim creation. It is that simple! If the world name is displayed in bold, it indicates that claim creation is disabled in that world. If it is not displayed in bold, claim creation is permitted in that world.**

**Please note that this feature is currently limited to blocking claim creation in general, but in the future, we plan to expand its capabilities to include the ability to block access for placing specific types of claims in specific worlds.**

**We hope that this feature proves helpful in streamlining your claim management process.**

<img src="https://i.imgur.com/Kmj1Wfv.png" width="" height=""><br>
<img src="https://i.imgur.com/wbymNiD.png" width="" height=""><br>
<img src="https://i.imgur.com/RvhpncD.png" width="" height=""><br><br><br>

# Coming from Another Claim Plugin?
**We understand that the process of switching to a new land claiming system can be daunting, especially when you have a substantial amount of existing data. That is why we are proud to offer our Import System, designed to facilitate the transfer of data from other claim plugins to our system.**

**Currently, we support import from ProtectionStones and EpicProtections, but we are always open to adding support for other plugins. If you have a request for a specific plugin, we welcome you to reach out to us via our Discord channel.**

**With our in-game Import System, the transition to our land claiming solution is a breeze. Simply select the plugin from which you wish to import data, initiate the import process, and allow our algorithm to do the rest. It is that simple.**

**We are confident that our Import System will make your transition to our land claiming solution a smooth and effortless experience. We hope you will consider choosing our plugin for your land management needs.**

*( **IMPORTANT:** As you consider using our importation system, we kindly remind you to prioritize the safety and stability of your server data. Before proceeding, it is essential that you create a backup of your server to ensure that any unintended consequences can be easily addressed. In the event that any technical issues arise during the importation process, our dedicated support team will be available to assist you in resolving the issue. However, please note that while we will strive to resolve any code-related problems, we may not be able to restore any data that may have been lost or damaged. By taking the precaution of creating a backup beforehand, you can ensure the security of your data and minimize any potential disruption to your server. Thank you for considering our importation system )*

<img src="https://imgur.com/5DP5dwP.gif" width="" height=""><br>
<br><br>

# API Usage
Coming soon...
