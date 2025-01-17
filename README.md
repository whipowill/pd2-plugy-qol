# Project Diablo 2

This repo includes my files for playing PD2 w/ PlugY and some minor game tweaks.

![Project Diablo 2](https://i.imgur.com/UequUwU.jpeg)

## Install

Copy and paste these files into your PD2 directory, then run ``PlugY.exe`` w/ ``-3dfx -direct -txt`` arguments.

## Modifications

Minor changes I've made:

- Moved Deckard Cain in Act 5 to stand by stash
- Changed/silenced some irritating character sounds
- Modded high rune drops to be less punishing

The rune drop mod has to be copy and pasted from the mods folder from the appropriate season into ``data/global/excel/``.

See the PD2 wiki [bugs](https://projectdiablo2.miraheze.org/wiki/Bugs) page a list of all the known bugs.

## Keyboard

This game is very clicky and you can quickly develop carpal tunnel syndrome.  To avoid this I wrote a [keyboard macro](https://github.com/whipowill/ahk-autoattack) that lets you hold down ``spacebar`` to move and attack.  This makes melee characters a lot easier to play.

## Loot Filter

Included in this repo is my custom loot filter.  I've spent quite a bit of time perfecting this!  I think it serves as a great loot filter for both new and old players.

- Bind ``+`` and ``-`` to adjust loot filter level
- Bind ``CAPLOCK`` to always show loot

| Image 1 | Image 2 |
|:-------:|:-------:|
| ![Alt text 1](https://i.imgur.com/Kxy59Gf.jpeg) | ![Alt text 2](https://i.imgur.com/wYXMpQl.jpeg) |

Features:

- Tasteful color scheme
- No information overload
- Icon system shows gear quality
- Armors show weight
- Charms show item level (for re-rolling)
- Rings and amulets show item level (for crafting)
- Runes show rune number (for organization)
- Sets show set number (for organization)
- Maps show difficulty level and standardize appearance
- Set and unique armor/weapons show upgrade recipies
- All armor/weapons show maximum sockets
- Special reagents show combination recipies
- Stackable gems show socket effects
- Computer generated loot filter codes ([Loot Filter Builder](https://github.com/whipowill/php-pd2-filter-builder))
	- Base items list all runewords possible
	- Tier labels on gear per your preferences (this version uses mine)

| Image 1 | Image 2 | Image 3 |
|:-------:|:-------:|:-------:|
| ![Alt text 1](https://i.imgur.com/BSPfIhV.jpeg) | ![Alt text 2](https://i.imgur.com/5qmgmHv.jpeg) | ![Alt text 3](https://i.imgur.com/gcXLIxg.jpeg) |

Levels:

- #1 - ``Hide Junk``
	- Hide low level potions
	- Hide gold (but you still pick up)
	- Hide non-necessary items like keys and quivers
	- Hide non-usable base armors/weapons for runewords like gloves, belts, and boots
	- Hide non-usable base armors/weapons for runewords like ``SOCK=1`` and ``INF``
	- Hide non-ideal base armors/weapons for runewords (this is subjective!)
		- Basically showing light armors, eth armors, class items, and good helms, shields, polearms, and swords
- #2 - ``Hide Junk, Magic``
	- Hide magic armors/weapons except elite craftable gloves, belts, and boots
- #3 - ``Hide Junk, Magic, Rare``
	- Hide rare armors/weapons except circlets, gloves, belts, and boots
- #4 - ``Hide Junk, Magic, Rare, Non-Tier``
	- Hide non-elite base armors/weapons for runewords
	- Only tier 1-5 gear drops will print in the chat
	- Only mid and high rune drops will print in the chat

You can read the ``default.filter`` file to see more information about how it's designed.  Most of the hiding instructions are at the very bottom of the file.  You can also search ``hide`` to find misc codes.

## Credits

- [BetweenWalls](https://github.com/BetweenWalls/PD2-PlugY) - initial PlugY files
- [SilverSix311](https://github.com/SilverSix311/PlugY-PD2) - fixing PlugY work on TCP/IP games
- [Bayaraa](https://github.com/bayaraa/d2gl/releases) - video driver ``glide3x.dll``
- [Jarcho](https://github.com/Jarcho/d2-rs/releases) - fps enhancement ``d2fps.dll``
- [Public Filters](https://wiki.projectdiablo2.com/wiki/Item_Filtering#List_of_Public_Filters) - recipie descriptions

## External Links

- [PD2 Website](https://www.projectdiablo2.com/) - official website
- [PD2 Wikipedia](https://projectdiablo2.miraheze.org/wiki) - official wiki
- [PD2 Runewizard](https://kvothed2.github.io/pd2-runewizard/) - handy runeword helper
- [PD2 Filter Rules](https://projectdiablo2.miraheze.org/wiki/Item_Filtering) - loot filter rules
- [D2 MPQEditor](http://www.zezula.net/en/mpq/download.html) - extract game TXT files
- [D2 ExcelPlus](https://github.com/Cjreek/D2ExcelPlus) - edit game TXT files
- [D2 AutoHotKey](https://github.com/whipowill/ahk-autoattack) - mouse auto-clicker
- [PD2 Loot Filter Builder](https://github.com/whipowill/php-pd2-lfb) - build your own tier list
- [D2 Armor Appearances](https://i.redd.it/qw4onikwxdx71.jpg) - see how armor looks
- [Arreat Summit](http://classic.battle.net/diablo2exp/items/basics.shtml) - info on the original game