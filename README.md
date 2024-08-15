# Project Diablo 2

This repo includes my files for playing PD2 w/ PlugY and some minor game tweaks.

![Project Diablo 2](https://i.imgur.com/UequUwU.jpeg)

## Install

Copy and paste these files into your PD2 directory, then run ``PlugY.exe`` w/ ``-3dfx -direct -txt`` arguments.

## Modifications

Changes I've made:

- Moved Deckard Cain in Act 5 to stand by stash
- Changed/silenced some irritating character sounds
- Modded rune drops to be less punishing

The rune drop mod has to be copy and pasted from the mods folder from the appropriate season into ``data/global/excel/``.

My notes about PlugY:

- DClone as added by PlugY won't drop Anni
- Shared gold must be disabled as it conflicts w/ PD2
- Option ``EnabledTXTFilesWhenMSExcelOpenIt`` doesn't seem to work

See the PD2 wiki [bugs](https://projectdiablo2.miraheze.org/wiki/Bugs) page a list of all the known bugs.

## Video

Some notes about video settings.

I instructed PlugY to load ``d2fps.dll``which is an extra library that works even better at motion prediction.  It requires that ``glide3x.dll`` (the D2GL video driver icluded with PD2) have motion prediction turned off.

I load this extra DLL thru PlugY instead of D2GL bc a) it works better that way, and b) you can still load normal PD2 to play online bc this extra DLL will cause PD2 to kick you.

Final note is the best video filter by far is ``4xbr-hybrid-crt``.

## Keyboard

This game is very clicky and you can quickly develop carpal tunnel syndrome.  To avoid this I wrote a [keyboard macro](https://github.com/whipowill/ahk-autoattack) that lets you hold down ``spacebar`` to move and attack.  This makes melee characters a lot easier to play.

## Loot Filter

Included in this repo is my custom loot filter.  I've spent quite a bit of time perfecting this!  I think it serves as a great loot filter for both new and old players.

- Bind ``+`` and ``-`` adjust loot filter level
- Bind ``CAPLOCK`` to always show loot

| Image 1 | Image 2 |
|:-------:|:-------:|
| ![Alt text 1](https://i.imgur.com/Kxy59Gf.jpeg) | ![Alt text 2](https://i.imgur.com/wYXMpQl.jpeg) |

Features:

- Tasteful color scheme
- No information overload
- Icon system shows item quality
- Armors show weight
- Rings and amulets show item level (for crafting)
- Runes show rune number (for organization)
- Sets show set number (for organization)
- Maps show difficulty level
- Base items list all runewords possible
- Weapons and armor show upgrade recipies
- Special items show combination recipies
- Stackable items show socket effects

| Image 1 | Image 2 | Image 3 |
|:-------:|:-------:|:-------:|
| ![Alt text 1](https://i.imgur.com/BSPfIhV.jpeg) | ![Alt text 2](https://i.imgur.com/5qmgmHv.jpeg) | ![Alt text 3](https://i.imgur.com/gcXLIxg.jpeg) |

Levels:

- Filter L1 - ``Hide Junk``
	- Hide low level potions
	- Hide gold (but you still pick up)
	- Hide non-necessary white items like keys and quivers
	- Hide non-usable white items like gloves, belts, and boots as well as inferior items
	- Hide non-ideal white items for runewords (this is subjective!)
- Filter L2 - ``Hide Junk, Magic``
	- Hide magic items except rings, amulets, charms, and elite craftable gloves, belts, and boots
- Filter L3 - ``Hide Junk, Magic, Rare``
	- Hide rare items except rings, amulets, quivers, gloves, belts, and boots
- Filter L4 - ``Hide Junk, Magic, Rare, Non-Tier``
	- Hide non-elite white items
	- Non-tier set and unique drops no longer print in the chat

You can read the ``default.filter`` file to see more information about how it's designed.  Most of the hiding instructions are at the very bottom of the file.

## Credits

- [BetweenWalls](https://github.com/BetweenWalls/PD2-PlugY) - initial PlugY files
- [Bayaraa](https://github.com/bayaraa/d2gl/releases) - video driver ``glide3x.dll``
- [Jarcho](https://github.com/Jarcho/d2-rs/releases) - fps enhancement ``d2fps.dll``
- [Public Filters](https://wiki.projectdiablo2.com/wiki/Item_Filtering#List_of_Public_Filters) - borrowed recipie descriptions

## External Links

- [PD2 Website](https://www.projectdiablo2.com/) - official website
- [PD2 Wikipedia](https://projectdiablo2.miraheze.org/wiki) - official wiki
- [PD2 Runewizard](https://kvothed2.github.io/pd2-runewizard/) - handy runeword helper
- [PD2 Filter Rules](https://projectdiablo2.miraheze.org/wiki/Item_Filtering) - loot filter rules
- [D2 MPQEditor](http://www.zezula.net/en/mpq/download.html) - extract game TXT files
- [D2 ExcelPlus](https://github.com/Cjreek/D2ExcelPlus) - edit game TXT files
- [Will Scarlet's D2 AutoHotKey](https://github.com/whipowill/ahk-autoattack) - mouse auto-clicker
- [Will Scarlet's PD2 Loot Filter Builder](https://github.com/whipowill/php-pd2-filter-builder) - build your own tier list