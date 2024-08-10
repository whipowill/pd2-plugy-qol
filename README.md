# Project Diablo 2

![PD2 PlugY QOL Mod Pack](https://i.imgur.com/JgWjLrw.jpeg)

This repo includes my files for playing PD2 w/ PlugY and some minor game tweaks.

## Install

Copy and paste these files into your PD2 directory, then run ``PlugY.exe`` w/ ``-3dfx -direct -txt`` arguments.

### Helpful Links

- [ProjectD2](https://www.projectdiablo2.com/) - official website
- [Wikipedia](https://projectdiablo2.miraheze.org/wiki) - official wiki
- [Runewizard](https://kvothed2.github.io/pd2-runewizard/) - handy runeword helper

## Modifications

Changes I've made:

- Moved Deckard Cain in Act 5 to stand by stash
- Changed/silenced some irritating character sounds
- Modded rune drops to be less punishing

The rune drop mod has to be copy and pasted from the mods folder from the appropriate season into ``data/global/excel/``.

Some notes about PlugY:

- You must have shared gold disabled as it conflicts w/ PD2
- The ``EnabledTXTFilesWhenMSExcelOpenIt`` option doesn't seem to work

See the PD2 wiki [bugs](https://projectdiablo2.miraheze.org/wiki/Bugs) page a list of all the known bugs.

### Helpful Links

- [MPQEditor](http://www.zezula.net/en/mpq/download.html) - for extracting game TXT files
- [D2ExcelPlus](https://github.com/Cjreek/D2ExcelPlus) - for editing game TXT files

## Video

Some notes about video settings.

I instructed PlugY to load ``d2gl.json``which is an extra library that works even better at motion prediction.  It requires that your D2GL have motion prediction turned off or it won't work right.

I run this extra DLL thru PlugY instead of thru D2GL bc a) it works better that way (flawless), and b) you can still load normal PD2 to play online bc this extra DLL would cause PD2 to kick you.

Final note is the best video filter by far is ``4xbr-hybrid-crt``.

### Helpful Links

- [D2GL](https://github.com/bayaraa/d2gl/releases/) - PD2 integrated graphics driver
- [D2FPS](https://github.com/Jarcho/d2-rs/releases) - extra DLL for superior motion prediction

## Keyboard

This game is very clicky and you can quickly develop carpal tunnel syndrome.  To avoid this I wrote a [keyboard macro](https://github.com/whipowill/ahk-autoattack) that lets you hold down ``spacebar`` to move and attack.  This makes melee characters a lot easier to play.

Additional Tips:

- Bind ``+`` and ``-`` adjust loot filter level
- Bind ``CAPLOCK`` to always show loot

## Loot Filter

Included in this repo is my custom loot filter.  It's a port from my vanilla D2 days that I've been working to make suitable for PD2.

Filter Levels:

- Hide Junk
- Hide Junk, Magic
- Hide Junk, Magic, Rare
- Hide Junk, Magic, Rare, Non-Tier

You can read the ``default.filter`` file to see more information about how it's designed.

### Helpful Links

- [Filter Rules](https://projectdiablo2.miraheze.org/wiki/Item_Filtering) - loot filter rules
- [PD2 Loot Filter Builder](https://github.com/whipowill/php-pd2-filter-builder) - build your own tier list

## Credits

Thanks to [BetweenWalls](https://github.com/BetweenWalls/PD2-PlugY) for the initial PlugY files I used in this repo.