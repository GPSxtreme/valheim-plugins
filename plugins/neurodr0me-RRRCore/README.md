# RRR Core

- If you would like to support the development of my mods, donations are much appreciated. Thank you! http://paypal.me/neurodr0me


- IMPORTANT! RRR Monsters and RRR NPCs are now INCLUDED in RRR Core. ***Remove RRRMonsters and RRRNpcs from your plugins folder!***


- **SERVER ADMINS: Custom mob textures cannot sync over the network. Your users must be provided with them before joining, otherwise they will only see the default textures.**

## Setup

Extract the zip file to your `Valheim\BepInEx` folder. Config files should end up in `Valheim\BepInEx\config`, everything else should end up in `Valheim\BepInEx\plugins`. Config files will also be generated automatically if missing.


## Help!

If you need further assistance, feel free to bug me in the Valheim Modding Discord at https://discord.gg/RBq2mzeu4z


## Changelog

### 3.1.5
- Fix "missing method FindChild" error from new Valheim update.~~~~

### 3.1.4
- Fix "key already added" error when exiting a world to the main menu with certain other mods installed.

### 3.1.3
- Fix for Valheim update 0.217.22.

### 3.1.2
- Fix "ProcessPlaceholders" crash that was preventing mobs from loading.

### 3.1.1
- Fix fatal error when loading into a world multiple times in one game session.

### 3.1.0
- Custom mob effects lists (e.g. death effects) and custom attack effects lists (e.g. on hit effects) can now always reference any other
    RRR npc or monster, no matter their name load order. This also allows for 'circular references', where mob A spawns mob B when it
    dies, and then mob B also spawns mob A when it dies.
- Custom mob *textures* will no longer try to sync online. Valheim's networking is just not suited for large file transfer. Attempting
    to do so was breaking ServerSync and causing other problems, while rarely working. Instead, textures can now load from your local
    configs directory, which they couldn't do before!
- **SERVER ADMINS: This means you must now include textures in your server pack. Custom mob (JSONs) will continue to sync normally.**
- Custom mob configs can now be named under the format "rrr.custom.*.json", and no longer require "monsters" or "npcs" after the RRR.
    Configs that use the old format will still be loaded normally too, so don't panic!

### 3.0.1
- Update to latest version of server sync.
- Fix NPCs using player bows firing very slow arrows. They still can't use monster bows, nor crossbows--still looking into that.

### 3.0
- Fixed for Hildir's Request.
- IMPORTANT! RRR Monsters and RRR NPCs are now INCLUDED in RRRCore. Remove RRRMonsters and RRRNpcs from your plugins folder!

### 2.15
- IronGate removed "m_tolerateFire" from Character so that field is now deprecated and will not do anything for custom monsters.

### 2.14
- Fixed config sync for servers.

### 2.13
- Updated for Valheim Mistlands.

### 2.12
- To Character, added bStaggerWhenBlocked.
- To CustomAttack, added fAIAttackRange, fAIAttackRangeMin, fAIAttackMaxAngle, bBlockable, bDodgeable, bForceAttackChainZero, bUseCharacterFacing, fAttackRange, fAttackHeight, fAttackRayWidth.