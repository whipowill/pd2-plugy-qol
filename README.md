# Project Diablo 2

The best way to play the game.

This repo includes my files for playing the game using PlugY w/ some minor game tweaks.  I moved Deckard Cain in Act 5 to stand by the stash and I modded ``TreasureClassEx.txt`` to make Countess drop better runes.

## Performance

Edit ``d2gl.json`` to use D2FPS:

```
"load_dlls_early": "d2fps.dll:stdcall:_Init@0",
```

## Notes

To my knowledge, there are no DLL mods that work other than PlugY.  This sadly excludes the legendary [BaseMod](https://d2mods.info/forum/viewtopic.php?t=65492).  Some additional notes:

- In PlugY, you must have shared gold disabled as it conflicts with PD2
- In PlugY, the ``EnabledTXTFilesWhenMSExcelOpenIt`` option doesn't seem to work

See the PD2 wiki [bugs](https://projectdiablo2.miraheze.org/wiki/Bugs) page to read more.

## External Links

- [ProjectD2](https://www.projectdiablo2.com/) - official website
- [Wikipedia](https://projectdiablo2.miraheze.org/wiki) - official wiki
- [Runewizard](https://kvothed2.github.io/pd2-runewizard/) - handy runeword helper
- [BetweenWalls](https://github.com/BetweenWalls/PD2-PlugY) - custom PlugY files
- [D2ExcelPlus](https://github.com/Cjreek/D2ExcelPlus) - for editing game TXT files
- [MPQEditor](http://www.zezula.net/en/mpq/download.html) - for extracting game TXT files
- [D2GL](https://github.com/bayaraa/d2gl/releases/) - graphics driver (check for updates)
- [D2FPS](https://github.com/Jarcho/d2-rs/releases) - motion prediction driver (check for updates)
- [Filters](https://projectdiablo2.miraheze.org/wiki/Item_Filtering) - loot filter rules