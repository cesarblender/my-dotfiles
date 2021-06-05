# My *Arch Linux* Dotfiles

In this file you'll find all my *Arch Linux* and my *Vim & NeoVim* configuration.

## Setup

- Clone this repository on any folder.
- Go to the "Dotfiles" folder.
- Copy the ".config" folder to your `$HOME` folder `cp -rf ./.config ~`.
- Copy the "background.jpg" file to `/usr/share/pixmaps/` `cp ./background.jpg /usr/share/pixmaps/`
- Install the following packages.

## Packages to install 

I'll asume that you have installed an AUR helper like yay.
``
$ pacman -S i3 ranger neofetch neovim firefox picom pcmanfm rofi alacritty pulseaudio git python3 dunst lxappearance
$ yay -S polybar
``
I recommend install lightdm because is very customizable.

`
$ pacman -S lightdm lightdm-gtk-greeter lightdm-gtk-settings
`
You can enable lightdm with `systemctl enable lightdm.service`

After enable lightdm you need to disable any other session manager.

# Theming

`
$ pacman -S papirus-icon-theme adapta-gtk-theme
$ yay -S nerd-fonts-meslo nerd-fonts-hack nerd-fonts-fira-code

# To change lightdm themes, icons, and typography run (with root)
$ lightdm-gtk-settings

# To change the pcmanfm icons & themes (without root)
$ lxappearance
`

