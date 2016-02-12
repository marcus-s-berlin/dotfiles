# dotfiles
A collection of the configuration files marcus-s uses. In here are configs for VIM, Awesome (WM), and many others. Please note that some files to be found in here are tailored to Arch Linux. You would have to perform modifications in certain files if used on a different distribution.

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

There are three buttons on the right, serving as the fast lane for shutdown, reboot, and logout. The user name display is only for decoration and has no effect. You can remove that widget, and/or the buttons, if you so like.

**IMPORTANT**: Change the folder on line 17 in rc.lua to the home folder location on your computer.

**NOTE**: Clicking on the Pacman icon, regardless of how many updates there are, will spawn a terminal asking you if you want to run `sudo pacman -Syu`.

**NOTE**: Clicking on either one of the buttons in the top for logout, restart, or shutdown, will have an immediate effect. You are not asked any questions, no prompts will show. **So save your stuff before clicking either one.** Like I said, it's a fastlane service.

## REQUIREMENTS:
For the `rc.lua` to work out of the box, you'd need some tools installed. They are as follows.

- Editor: **gvim** (Graphical version of VIM, install with `pacman -S gvim`)
- Terminal: **lilyterm** (lightweight but feature-rich terminal, install with `pacman -S lilyterm`)
- Battery widget: Requires the tool `acpi` to be installed. Get it with `pacman -S acpi`

Of course feel free to either edit the file to suit your needs, or alter to the tools you use.

## .vim :
Contains my personal plugin setup that I use for my daily editing with VIM. The vimrc file in that folder is the .vimrc file I use which is normally located in the home folder.
