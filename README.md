# dotfiles
A collection of the configuration files marcus-s uses. In here are configs for VIM, Awesome (WM), and many others.

## .config/awesome :
Contains my personal setup for the Awesome 3.5 window manager. Comes with a volume and Pacman widget. This config is tailored specifically to Arch Linux. However, it is possible to easily augmentize it for your needs. Make sure to read through the pages over at http://awesome.naquadah.org .

It comes with a theme and icons I have developed myself, named after the machine I use it on. Hence the name "MarcBookPro". You can of course augmentize this at will. Additionally the rc.lua file has been tweaked to have some extra keybindings. They are as follows:

- Mod4 + F12: Increase volume
- Mod4 + F11: Decrease volume
- Mod4 + F10: Unmute
- Mod4 + F9: Mute
- Mod4 + F1: Decrease brightness (Laptops only)
- Mod4 + F2: Increase brightness (Laptops only)

Of course the last two won't have any effect on normal desktop computers. The sound widget uses the ALSA system, which is the most common on Linux systems.

Further some parts have been split up into smaller .lua files, so that things can be changed more quickly and easily. The files and their contents should be self-explanatory.

IMPORTANT: Change the folder on line 17 in rc.lua to the home folder location on your computer.


## .vim :
Contains my personal plugin setup that I use for my daily editing with VIM. The vimrc file in that folder is the .vimrc file I use which is normally located in the home folder.
