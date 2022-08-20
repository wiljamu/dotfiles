# dotfiles
me hyprland dotfiles


# Installation

## Install Paru & Base-Devel

```
sudo pacman -S --needed base-devel
git clone https://aur.archlinux.org/paru.git
cd paru
makepkg -si
```

## Make Wayland Work

- Add 'nvidia_drm.modeset=1' to the end of the 'options' line 
