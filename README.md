# dotfiles
My Arch Linux configuration (i3wm, pcmanfm, polybar, neovim)

You can use this files on any linux distribution (that you can open a terminal), you can install all the dependencies below and start using a tiling window manager.

## Firstly, install the dependencies below (you can use any package manager, like pacman, apt, apk, etc.)

$ `pacman -S i3 polybar pcmanfm neovim rofi feh picom compton terminator`

optional you can install a session manager (LightDM)

$ `pacman -S lightdm lightdm-gtk-greeter lightdm-gtk-greeter-settings`

## Now, we must to install other files

If you're running on Arch or another minimal linux distro, you must install an font manager

$ `pacman -S font-manager`

and then enter to the Hack Nerd Font folder and install theese font files (if you don't know how to do it with the terminal, only click on all the files and click install)

you should move your wallpaper to your user directory ($HOME or ~/), then rename it for bg.jpg

or copy my wallpaper with this command

$ `cp ./bg.jpg $HOME/`

## Then copy this files with theese commands

$ `cp -r ./i3 $HOME/.config/`

$ `cp -r ./rofi $HOME/.config/`

$ `cp -r ./rofi $HOME/.config/`

Finally you must to logout from your window manager or restart your computer, then you'll select wich window manager you want to use select i3

## Note if you have an issue, go to this repository and add it, I'll fix your issues!

# Usual issues

## Polybar doesn't run?

only copy this command:

$ `sudo chmod -x $HOME/polybar/lauch.sh`

## The audio is muted

only copy this command:

$ `pacman -S pulseaudio`

and click on the volume module in polybar

## My background is png, what I can do?

go to google and search transform png to jpg and transform it!

## My keyboard layout is built in spanish and the settings're in english

try to restart your computer, if that doesn't work, edit the configuration file in i3

`nvim $HOME/i3/config`

and search the line `exec setxkbmap -layout es`, then change for your keyboard layout (search info on google!)