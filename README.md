Haven City Air Support
Version: 0.1.0

What this mod does
------------------
Haven City Air Support makes the late-game Haven City invasion feel more like an active citywide battle.

During the Metal Head attack on Haven City:
- Krimzon Guard bikes can spawn as part of the defense.
- Krimzon Guard Hellcats can spawn in the invasion state.
- KG bikes and Hellcats chase nearby Metal Heads at higher speed instead of only drifting through traffic.
- KG bikes and Hellcats fire at Metal Heads on the ground.
- When Jak pilots a KG bike or Hellcat, the mounted gun can auto-aim at nearby enemies while firing.
- City guard turrets that normally engage during zoomer pursuit can also stay active during the invasion and target Metal Heads.

Requirements
------------
- Windows
- OpenGOAL Launcher with Jak II installed and extracted
- A working Jak II OpenGOAL build

This installer was built and tested against the OpenGOAL official v0.3.3 Jak II layout.

Installation
------------
1. Extract this zip folder.
2. Double-click "Install Haven City Air Support.cmd".
3. When the wizard asks for your Jak II/OpenGOAL directory, choose your OpenGOAL folder.
   The most common choice is the folder that contains "OpenGOAL-Launcher.exe".
   The wizard also accepts the "active\jak2" folder or the "active\jak2\data" folder.
4. Confirm the detected Jak II data path and compiler path.
5. Let the installer patch the source files and rebuild Jak II. This can take a few minutes.
   The installer window should show status while the rebuild runs.
   On some Windows systems, the small installer window may briefly turn white or say "Not Responding" during the heavier parts of the install. Do not be alarmed and do not close it. The installer should still work as expected; wait for the success popup or an error popup.
6. After the installer finishes, it creates an installed mod folder at:
   features\jak2\mods\JakMods\haven-city-air-support
7. That installed mod folder contains the README, metadata, an install summary, and a configured "Launch Haven City Air Support.vbs" file.
8. Double-click "Launch Haven City Air Support.vbs" from the installed mod folder to launch Jak II with the rebuilt modded data.
9. You can also use the configured VBS file in the extracted installer folder if you prefer.
10. Load a late-game Haven City invasion save to see the changes.

Launching from the VBS file
---------------------------
The included "Launch Haven City Air Support.vbs" starts as a placeholder. Run the installer first.

After installation, the wizard creates a configured VBS launcher inside:
features\jak2\mods\JakMods\haven-city-air-support

The wizard also rewrites the VBS file in the extracted installer folder with your actual OpenGOAL paths. From then on:
1. Double-click "Launch Haven City Air Support.vbs".
2. A command window should not stay open; the VBS launches the game quietly in the background.
3. Load a save where Haven City is in the late-game Metal Head invasion state.

The VBS launcher uses its own mod config folder. The main Air Support installer does not copy, overwrite, or seed any Jak II save files. If your save list is empty when launching through the VBS, either copy saves manually or use the optional save overwrite installer below.

If the VBS launcher does not work on your system, launch Jak II normally through OpenGOAL Launcher after installing. The installer patches and rebuilds your local Jak II data, so the modded behavior should still be present.

Included personal saves
-----------------------
This zip includes a "personal-saves" folder with a Jak II OpenGOAL save set:
personal-saves\OpenGOAL\jak2\saves\BASCUS-97265AYBABTU!

Game 3, the third save slot, is a late-game Haven City invasion state save. Use that save to test the mod's Krimzon Guard vehicle, Hellcat, and turret support behavior.

The main Air Support installer does not install these bundled saves automatically. They are included only so the user can install them deliberately with the optional save overwrite installer below.

Optional save overwrite installer
---------------------------------
If you want to replace your current Jak II OpenGOAL saves with the included invasion-state save set, double-click:
Install Included Invasion Save.cmd

This is separate from the main mod installer. It overwrites the Jak II save banks in your normal OpenGOAL profile with the bundled saves, but it creates a timestamped backup first if saves already exist.

The save installer can also ask for your OpenGOAL folder so it can overwrite the mod VBS launcher's isolated save folder too. Choose that option if you launch the mod through "Launch Haven City Air Support.vbs".

Do not run the save overwrite installer unless you want the included saves to replace the saves currently shown by OpenGOAL Jak II.

What the installer changes
--------------------------
The installer patches source files in your own OpenGOAL Jak II install, then rebuilds the game output locally. It does not include or distribute Jak II game data.

The installer creates a timestamped backup before changing anything:
active\jak2\data\_mod_backups\haven-city-air-support\<timestamp>

Included source code
--------------------
This zip includes a "source-code" folder for Git hosting and review.

The "source-code\scripts" folder contains the installer, launcher, save installer, and package assembly scripts.

The "source-code\patches" folder contains a unified GOAL patch showing the OpenGOAL Jak II source edits made by the mod.

To uninstall or restore
-----------------------
You can restore the backed-up files by copying them from the backup folder back into your Jak II data folder, then rebuilding Jak II again.

You can also reinstall or repair Jak II through OpenGOAL Launcher to return to a clean build.

Disclaimer
----------
This is a fan-made gameplay mod and is not affiliated with Naughty Dog, Sony, or the OpenGOAL team.

The mod is stable and playable in testing, but there are minor bugs. Vehicle AI can occasionally behave strangely, combat can get busy, and some edge cases may depend on your save state or OpenGOAL version.

This mod is designed for and only meaningfully works during the late-game Haven City invasion state where Metal Heads attack the city. If you load an earlier story state, most of the modded combat behavior may not appear.

Back up important saves before using mods.
