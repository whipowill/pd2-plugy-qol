# Project Diablo II

These are my files for playing singleplayer [PD2](http://projectdiablo2.com).

## Features

- [PD2](https://wiki.projectdiablo2.com/wiki/Patch_Notes) - all the greatness of Project Diablo II
- [PlugY](http://plugy.free.fr/en/index.html) - adds 10 pages of shared stash and shared gold
- [D2DX](https://github.com/bolrog/d2dx/releases) - wildly improves framerate for singleplayer

I've also relocated Deckard Cain in Act 5 to stand beside the waypoint.

## Install

- Download PD2 using the official installer
- Rename ``C:\Path\To\Diablo II\ProjectD2\D2HD.dll`` to ``D2HD_unused.dll``
- Rename ``C:\Path\To\Diablo II\ProjectD2\Glide3dx.dll`` to ``Glide3dx_unused.dll``
- Copy/paste the files from this repository into the ``C:\Path\To\Diablo II\ProjectD2\`` directory
- Run the game using a shortcut w/ ``C:\Path\To\Diablo II\ProjectD2\Plugy.exe -3dfx -direct -txt`` as the target

## Bugs

The shared gold in PlugY just doesn't work.  If you're going to use it, use it quickly between characters and otherwise avoid it.  Anything you leave in there will eventually be lost.  I could never figure out why, even when I used different ``BH.dll`` files from SlashDiablo.  Something about PD2 using memory locations that are also used by PlugY.  Frustrating!

## Credits

- PD2 by Project Diablo II
- Plugy by Yohann
- D2DX by Balrog
- BH by Slash Diablo