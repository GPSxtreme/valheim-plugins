# Changelog

### 1.3.3 (Update brought to you by Azumatt)
- Remove the patcher and pre-patch the dll for you. Since modifications in memory caused issues with the AzuAnticheat (rightfully so), that I didn't account for.
- Move the changelog to the changelog tab/file.
- Fix up the README file to remove redundancy. While doing so, I noticed Rae's Distribution notice. This essentially gives me permissions to work on this mod more directly. Expect some updates soon that aren't external dll patching.
- Note:
    In my tests, the patchers folder was removed automatically when downloading this version, so you shouldn't have to remove manually. If you're experiencing issues, check there first.
    Additionally, as of right now I'm patching the dll and making the needed changes externally as a way to prevent having to rebuild this mod's assets. Though, as stated above, it appears I can take a more hands on approach without his permission. I'll be doing that soon, especially since I can keep his name and update in-place.

### 1.3.1/1.3.2 (Update brought to you by Azumatt)
- Un-deprecate the mod.
- Add OdinArchitectVersionPatcher to BepInEx/patchers folder to show correct version in chainloader.
- Add OALanternFix to fix the issues people were having with the surtling lanterns.

### 1.3.0
- Updated for latest version (Ashlands update)
- Updated Jotunn and core libraries

### 1.2.7
- Changed the chests size to don't exceed player inventory slots
- Reduced Bronze Storages size to 6/4 and 6/3
- Reduced Iron Storages size to  8/4 and 8/3
- Reduced Storage Decors sizes to 6/3 (Crates and Barrels)
- Duplicated StoneMarble column should be fixed now, it's vertical
- Changed all the "StoneMarble" pieces material type from stone back to marble. This should improve structural integrity and pieces crumbling.
- Changed the Stone Chisel layer for item which repair auto-pickup of it.
- Reduced storages costs by half - metals cost.
- Reduced storages visual size and fixed a bit snappoints, they should fit better for now
- Added configs for rows and columns of each container. Barrels and Crates are sharing the settings as they're same size. Storages have separated settings.
- Fixed some NRE problems for LODs of containers and pieces.

### 1.2.6
- Fixed AntiTroll Sharpstakes Wear'n'Tear, again and finally
- Changed big wooden floors wood type from normal wood to hard wood

### 1.2.5
- Updated for latest game version
- Updated for latest Jotunn version
- Fixed localization issues with some stone pieces
- Root folder is now `plugins` like before. Should fix installing this mod with ModManagers.
- Fixed AntiTroll Sharpstakes Wear'n'Tear
- Fixed Stone Wall Cross 26 Wear'n'Tear
- Tweaked Stone Marble pieces Wear'n'Tear (i think so)
- This mod will be not compatible with Valheim+