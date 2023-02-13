<img src="https://github.com/PearlLabTeam/PearlClaim/blob/main/images/smallers-logo.png" width=1500 height=700>

## Introduction
PearlClaim is the premier land claiming plugin for your server, offering advanced features and complete control over your lands. With our user-friendly, advanced GUI, you can easily edit everything in-game. Despite being in beta mode, we are dedicated to improving the plugin and making it the best it can be. Any feedback and bug reports are welcome and will be addressed promptly. Experience the ultimate in land claiming technology and secure your lands with PearlClaim today.

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
- [Adding Storages to Claims]()
- [Blacklist Worlds]()
- [Coming from Another Claim Plugin]()
- [API Usage]()

## Note
Please note that PearlClaim is currently in beta mode and may contain some bugs. If you encounter any difficulties, we encourage you to reach out to us on our discord server, where we will be more than happy to assist you and resolve any issues. Thank you for your understanding and support as we continue to improve and enhance the functionality of PearlClaim.

## Commands and Permissions
Here is a list of available commands and their respective permissions in PearlClaim:

| Command                                       | Description                                                                                                                      | Permission           |
|-----------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|----------------------|
| /claim                                        | Open the config menu of a claim if standing in one                                                                               | claim.use            |
| /claim create                                 | Create a claim from your stored claims (if any)                                                                                  | claim.create         |
| /claim edit                                   | Open the config menu of a claim if standing in one                                                                               | claim.edit           |
| /claim flags                                  | Open the flags GUI of the claim you're standing on                                                                               | claim.flags          |
| /claim storage                                | Open the storages that you have available in your claim                                                                          | claim.storage        |
| /claim delete                                 | Delete the claim you're standing on                                                                                              | claim.delete         |
| /claim store                                  | Pick up and store the claim you're standing on                                                                                   | claim.store          |
| /claim members < + / - > < player >           | Add or remove the given player into the claim you're standing on                                                                 | claim.modify.members |
| /claim role < member/admin >                  | Modify the member or admin roles from the claim you're standing on                                                               | claim.modify.roles   |
| /claim admin                                  | Open the Admin Configuration GUI                                                                                                 | claim.admin          |
| /claim admin giveclaim < player > < claimID > | Give the target player the claim with the provided ID                                                                            | claim.admin          |
| /claim admin import                           | Import the claims data from EpicProtections/Protection Stones (if you want us to add more plugins please let us know on discord) | claim.admin          |
| /claim admin reload                           | Reload every file and configuration and recreate files that are missing                                                          | claim.admin          |


## General Configurations
Some general configurations that are available to admins include:
<br><br><br>

### Selection Outline
The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.

<img src="https://i.imgur.com/PSh4yki.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

### Default Claims toggle
The "Default Claims toggle" option provides administrators with the ability to regulate the automatic generation of claims for new players upon joining the server. When enabled, if PearlClaim does not detect a player data file for a new player, it will generate one and automatically add the default claims defined within the system. This function enables a seamless and efficient claim generation process for new players.

<img src="https://i.imgur.com/jDVTBQO.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

### Language Switching
This feature provides the ability for administrators to switch between multiple languages, ensuring that the plugin interface and related messages are displayed in the preferred language selection.

<img src="https://i.imgur.com/X6VJuIA.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

### Claim Storage toggle
This option provides administrators with the ability to control the storage access of all claims within the system. When the storage option is set to "Disabled," it will restrict player access to all stored claims without impacting the actual content of the stored data.

<img src="https://i.imgur.com/JYwc76w.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

### Claim Storage Require Permission
This option determines the requirement for players to have a specific permission in order to access the storage through the graphical user interface (GUI). When set to "required," players must possess the specified permission in order to generate the storage in the GUI. On the other hand, if set to "not required," players will be able to see the storage button in the GUI even without the permission. However, it is important to note that this setting does not affect the player's ability to actually access the storage's contents, which will still require the specified permission.
<img src="https://i.imgur.com/ty2frbx.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

*All of these configurations can be easily modified from the plugin's settings menu, making it quick and simple for admins to get the plugin configured exactly how they want it.*
<br><br><br>
# Creating and Configuring Claims
Creating and modifying claims has never been simpler. PearlClaim offers an in-game claim creation system for server administrators, providing a more intuitive and user-friendly approach compared to other plugins that require manual modification within configuration files. To create a new claim, simply navigate to the Claims Editor GUI by clicking the "Claims Editor" button within the Admin Configuration and then select the "Create a Claim" button. When it comes to modifying a specific claim, simply click on it to access another GUI containing a range of customization options.

### Default Claim
This option allows administrators to set the claim as default, meaning it will be added to new players' stored claims upon joining.

<img src="https://i.imgur.com/iUWQZlT.png" width="" height="">
<br><br>The option can be easily modified through a simple click, as shown in the accompanying image. This intuitive and straightforward process makes it quick and effortless for administrators to adjust the setting according to their preferences.
<br><br><br>

### Modify Storage
This option opens a separate GUI that enables the modification of the claim's storage settings. Additional information can be found in the "Creating and Configuring Claims" section.

<img src="https://i.imgur.com/IKpKddo.png" width="" height="">

***Claim's Storage Editor***

<img src="https://i.imgur.com/C5VyhJe.png" width="" height="">
<br><br><br>

### Give to Player
Allows administrators to transfer the claim to another player by specifying the player's name in chat. It is important to note that any updates made to the claim after it has been transferred will not be reflected in the recipient player's stored claims.

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
If set to **UPGRADABLE,** you will need to provide values for per-block-upgrade-cost and max-upgrade-radius for all X,Y, and Z

<img src="https://i.imgur.com/iDlBA46.png" width="" height=""><br><br>
<img src="https://i.imgur.com/FiEz2wz.png" width="" height=""><br><br>

### Creation Prompt Block
Specifies the animation block that will accompany the player when selecting land to claim. This block will indicate the center point of the claim.

<img src="https://i.imgur.com/8nup5YJ.png" width="" height=""><br><br>
***When activated, this button will initiate the opening of a new graphical user interface with multiple pages. Within this interface, the user will have the ability to select the material of the animation item.***

<img src="https://i.imgur.com/WpP8qtD.png" width="" height=""><br>

### Delete
Deletes the claim and all its configurations.

<img src="https://i.imgur.com/PqwY4Ub.png" width="" height=""><br>

### Back
Returns to the main menu.

<img src="https://i.imgur.com/WxAbeBL.png" width="" height=""><br>
