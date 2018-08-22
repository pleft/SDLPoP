# SDLPoP
An open-source port of Prince of Persia, based on the disassembly of the DOS version.

More info: doc/Readme.txt


## To build for GameShell

1. `ssh` to GameShell
2. on home directory `/home/cpi/`:
   ```
   sudo apt-get install libsdl2-image-dev
   git clone https://github.com/pleft/SDLPoP.git
   cd SDLPoP
   cd src
   make all
   ```
3. If compilation succeeds, in `SDLPoP/` directory there should be an executable file named `prince`

```
cd /home/cpi/SDLPoP
ls
data/  doc/  mods/  prince  README.md  SDLPoP.ini  src/
```

4. Create a launcher shortcut for prince executable to be able to launch it through the GameShell's menu

```
echo /home/cpi/SDLPoP/prince full > /home/cpi/apps/launcher/Menu/GameShell/Prince.sh
chmod +x /home/cpi/apps/launcher/Menu/GameShell/Prince.sh
```

5. Reboot GameShell and start Prince Of Persia by selecting the Prince icon

## GameShell Controls

* `START` = Enter, make selection
* `MENU` = ESCape
* `LEFT`: turn or run left
* `RIGHT`: turn or run right
* `UP`: jump or climb up
* `DOWN`: crouch or climb down
* `A`: pick up things
* `A`+`LEFT`/`RIGHT`: careful step
