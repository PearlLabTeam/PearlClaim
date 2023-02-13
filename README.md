<img src="https://github.com/PearlLabTeam/PearlClaim/blob/main/images/smallers-logo.png" width=1500 height=700>

## Introduction
PearlClaim is the premier land claiming plugin for your server, offering advanced features and complete control over your lands. With our user-friendly, advanced GUI, you can easily edit everything in-game. Despite being in beta mode, we are dedicated to improving the plugin and making it the best it can be. Any feedback and bug reports are welcome and will be addressed promptly. Experience the ultimate in land claiming technology and secure your lands with PearlClaim today.

## Dependencies
The following must be installed for PearlClaim to function properly:
- Vault.jar
- An economy plugin
- A permissions plugin

Some popular permissions plugins include:
- LuckPerms
- UltraPermissions

## Table of Contents
- [Commands and Permissions](https://github.com/PearlLabTeam/PearlClaim/blob/main/README.md#Commands-and-Permissions)
- Permissions
- General Configurations
- Creating and Configuring Claims
- Adding Storages to Claims
- Blacklist Worlds
- Coming from Another Claim Plugin
- API Usage

## Note
Please note that PearlClaim is currently in beta mode and may contain some bugs. If you encounter any difficulties, we encourage you to reach out to us on our discord server, where we will be more than happy to assist you and resolve any issues. Thank you for your understanding and support as we continue to improve and enhance the functionality of PearlClaim.

## Commands and Permissions
Here is a list of available commands and their respective permissions in PearlClaim:

| Command                                       | Description                                                                                                                      | Permission    |
|-----------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|---------------|
| /claim                                        | Open the config menu of a claim if standing in one                                                                               | claim.use     |
| /claim create                                 | Create a claim from your stored claims (if any)                                                                                  | claim.create  |
| /claim edit                                   | Open the config menu of a claim if standing in one                                                                               | claim.edit    |
| /claim flags                                  | Open the flags GUI of the claim you're standing on                                                                               | claim.flags   |
| /claim storage                                | Open the storages that you have available in your claim                                                                          | claim.storage |
| /claim delete                                 | Delete the claim you're standing on                                                                                              | claim.delete  |
| /claim store                                  | Pick up and store the claim you're standing on                                                                                   |               |
| /claim members < + / - > < player >           | Add or remove the given player into the claim you're standing on                                                                 |               |
| /claim role < member/admin >                  | Modify the member or admin roles from the claim you're standing on                                                               |               |
| /claim admin                                  | Open the Admin Configuration GUI                                                                                                 |               |
| /claim admin giveclaim < player > < claimID > | Give the target player the claim with the provided ID                                                                            |               |
| /claim admin import                           | Import the claims data from EpicProtections/Protection Stones (if you want us to add more plugins please let us know on discord) |               |
| /claim admin reload                           | Reload every file and configuration and recreate files that are missing                                                          |               |
