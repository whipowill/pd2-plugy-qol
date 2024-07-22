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

Some notes about video settings.  I instructed ``d2gl.json`` to use the extra library D2FPS for best performance.  This is an optional upgrade included in D2GL.

```
"load_dlls_early": "d2fps.dll:stdcall:_Init@0",
```

Note that this added DLL will cause PD2 to block you from playing online. Final note is the best video filter by far is ``4xbr-hybrid-crt``.

### Helpful Links

- [D2GL](https://github.com/bayaraa/d2gl/releases/) - graphics driver (check for updates)
- [D2FPS](https://github.com/Jarcho/d2-rs/releases) - motion prediction driver

## Keyboard Macros

This game is very clicky and you can quickly develop carpal tunnel syndrome.  To avoid this I wrote a [keyboard macro](https://github.com/whipowill/ahk-autoattack) that lets you hold down ``spacebar`` to move and attack.  This makes melee characters a lot easier to play.

## Loot Filter

Included in this repo is my custom loot filter.  It's a port from my vanilla D2 days w/ some tweaks to make it work for PD2.

### Helpful Links

- [Filter Rules](https://projectdiablo2.miraheze.org/wiki/Item_Filtering) - loot filter rules

## Credits

Thanks to [BetweenWalls](https://github.com/BetweenWalls/PD2-PlugY) for the initial PlugY files I used in this repo.