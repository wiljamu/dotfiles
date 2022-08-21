# dotfiles
me hyprland dotfiles


# Installation

## Install Paru & Base-Devel + Git

```
sudo pacman -S --needed git base-devel
git clone https://aur.archlinux.org/paru.git
cd paru
makepkg -si
```


## Make Wayland Work

If using systemD boot else refer to https://wiki.archlinux.org/title/Kernel_parameters
- Add `nvidia_drm.modeset=1` to the end of the `options` line in `/boot/loader/entries/arch.conf`.

- Edit `/etc/mkinitcpio.conf` and add `nvidia nvidia_modeset nvidia_uvm nvidia_drm` in the parenthesis of `MODULES=()`

- Update kernel headers with 
```
sudo mkinitcpio -P
```

- Reboot


## Install Hyprland & Dots

```
git clone https://github.com/wiljamu/dotfiles.git
cd dotfiles
sudo chmod +x install
install
```

