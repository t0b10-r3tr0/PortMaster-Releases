# PortMaster Releases

## Bind Mount Fix for exFAT FS (Knulli, Batocera)

In order to support the exFAT file system on [Knulli](https://knulli.org/) and [Batocera](https://batocera.org/), a new core function was added to PortMaster (`bind_directories`) to replace the previous method of using symbolic links. This resulted in many ports getting updated which now need to be tested. For status and progress, check our [**Discord Testing Thread**](https://discord.com/channels/1122861252088172575/1315085237788868608)

### Installation Instructions:

The instructions will apply to **all** of the ports tested in this post:
1. If you have the port already, uninstall it through PortMaster GUI: Manage Games > Game Info > Uninstall. 
2. Copy the `.zip` file to the `autoinstall` directory within the [PortMaster directory for your device](https://portmaster.games/installation.html#via-zip).
  * Option 1: Use SMB, SSH, or any other method provided by your CFW
  * Option 2: If your device supports it, remove micro-sd from device and copy files with computer
4. Start PortMaster and allow the auto-installation to continue.
5. Quit PortMaster and restart EmulationStation or your device.
6. Launch the port from the Ports section of ES.

#### Important

You must replace the `funcs.txt` within your PortMaster directory with the one contained in this repository. It is recommended that you back that version u prior to replacing.

### Testing

The port must be tested on the following fimwares to be considered as a passed test:
- Knulli
- Any other PM-supported CFW (ArkOS, ROCKNIX, AnberELEC, etc.)

In order consider the test passed for your device / CFW combo the following conditions must be satisfied:

1. The port loads without issue, even after rebooting the device.
2. The saves/settings persist, even after rebooting the device.
3. If port was installed previously, the existing saves/settings were preserved when testing the new version.

### Affected Ports

This repository contains all of the ports that have been affected as a result of these changes. The symbolic linking logic has has been replaced with PM's `bind_directory`, which require testing. This is a complete listing of the affected ports needing testing. To download the whole collection, [**click this link**](https://github.com/t0b10-r3tr0/PortMaster-Releases/archive/refs/heads/main.zip). To downoad an individual port, navigate to the appropriate directory, then the corresponding `.zip` file, and click the button titled *Download raw file*.

#### Ready to Run:

* Abes Adventure
* Abuse
* Armagetron Advanced
* Asylum
* Blobwars
* Block Attack
* Blockout 2
* Bos Wars
* C-Dogs
* Cave Story-evo
* Descent 2
* Descent
* Don Ceferino Hazaña
* Flare Engine
* FreeSiege
* Freedroid
* Gigalomania
* Grafx2
* Heroes
* Hex-A-Hop
* Hocoslamfy
* Holotz Castle
* Hydra Castle Labyrinth
* LieroLibre
* Marathon 2
* Marathon Infinity
* Marathon
* Meritous
* OpenTyrian
* Openomf
* Penguin Command
* Rise of the Triad - The Hunt Begins
* Rockdodger
* Rocks n Diamonds
* Shippy
* Super Transball 2
* VVVVVV
* Wolfenstein 3D

#### Game Files Required

* Air
* Alien vs Predator
* Angband
* Anodyne
* Axiom Verge
* Bleed
* Bleed2
* Blood
* Blossom Tales II
* Celeste
* Chasm
* Clannad Tomoyo After
* Clannad
* Daikatana
* Descent 3
* Duke3D - Alien World Order
* Exhumed
* Fheroes2
* Freesynd
* Hexen 2 - Portal of Praevus
* Hexen 2
* Hurrican
* If On A Winter's Night, Four Travelers
* Kanon
* Little Busters!
* Mystik Belle
* NAM
* Need For Speed II SE
* PanzerPaladin
* Planetarian
* Quake 3
* Redneck Rampage Rides Again
* Redneck Rampage
* Return to Castle Wolfenstein
* RigelEngine
* Rise of the Triad - Dark War
* Shipwreck
* Shovel Knight
* Sonic 3 AIR
* Star Wars Jedi Knight - Jedi Academy
* Star Wars Jedi Knight II - Jedi Outcast
* SteelAssault
* Timespinner
* Tomb Raider 1
* TowerFall Ascension
* World War II GI
* World of Goo

### Contributing

You can download the ports to your device and join us in the [Discord testing thread](https://discord.com/channels/1122861252088172575/1315085237788868608) to check the current status of the testing progress. 