# Project Diablo 2

![PD2 PlugY QOL Mod Pack](https://i.imgur.com/JgWjLrw.jpeg)

This repo includes my files for playing PD2 w/ PlugY and some minor game tweaks.

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

I instructed PlugY to load ``d2fps.json``which is an extra library that works even better at motion prediction.  It requires that ``d2gl.dll`` (which is icluded with PD2) have motion prediction turned off.

I load this extra DLL thru PlugY instead of D2GL bc a) it works better that way, and b) you can still load normal PD2 to play online bc this extra DLL will cause PD2 to kick you.

Final note is the best video filter by far is ``4xbr-hybrid-crt``.

## Keyboard

This game is very clicky and you can quickly develop carpal tunnel syndrome.  To avoid this I wrote a [keyboard macro](https://github.com/whipowill/ahk-autoattack) that lets you hold down ``spacebar`` to move and attack.  This makes melee characters a lot easier to play.

## Loot Filter

Included in this repo is my custom loot filter.  It's a port from my vanilla D2 days that I've been working to make suitable for PD2.  I've spent quite a bit of time perfecting this!

- Bind ``+`` and ``-`` adjust loot filter level
- Bind ``CAPLOCK`` to always show loot

Filter Levels:

- Filter Level 1 - ``Hide Junk``
	- Hide low level potions
	- Hide gold (but you still pick it up)
	- Hide unusable white items like gloves, belts, and boots as well as inferior items
	- Hide non-ideal white items that are NOT class items, kite shields, polearms, big swords, and light armors
- Filter Level 2 - ``Hide Junk, Magic``
	- Hide all magic items except rings, amulets, charms, and elite craftable gloves, belts, and boots
- Filter Level 3 - ``Hide Junk, Magic, Rare``
	- Hide all rare items except rings, amulets, quivers, gloves, belts, and boots
- Filter Level 4 - ``Hide Junk, Magic, Rare, Non-Tier``
	- Hide non-elite white items
	- Non-tier set and unique items still drop, but no longer print in the chat

The loot filter will ALWAYS show:

- Level appropriate potions
- Light armors ideal for runewords, as well as common weapons
- Elite ethereal armors ideal for mercenary runewords
- Magic rings, amulets, charms, and elite craftable gloves, belts, and boots
- Rare rings, amulets, quivers, gloves, belts, and boots
- Set and unique items

You can read the ``default.filter`` file to see more information about how it's designed.

## Credits

Thanks to [BetweenWalls](https://github.com/BetweenWalls/PD2-PlugY) for the initial PlugY files I used in this repo.

### External Links

- [PD2 Website](https://www.projectdiablo2.com/) - official website
- [PD2 Wikipedia](https://projectdiablo2.miraheze.org/wiki) - official wiki
- [PD2 Runewizard](https://kvothed2.github.io/pd2-runewizard/) - handy runeword helper
- [PD2 Filter Rules](https://projectdiablo2.miraheze.org/wiki/Item_Filtering) - loot filter rules
- [D2 MPQEditor](http://www.zezula.net/en/mpq/download.html) - extract game TXT files
- [D2 ExcelPlus](https://github.com/Cjreek/D2ExcelPlus) - edit game TXT files
- [whipowill's D2 AutoHotKey](https://github.com/whipowill/ahk-autoattack) - mouse auto-clicker
- [whipowill's PD2 Loot Filter Builder](https://github.com/whipowill/php-pd2-filter-builder) - build your own tier list