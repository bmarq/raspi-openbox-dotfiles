# raspi-openbox-dotfiles
## Preview
### Based on debian openbox/fluxbox dotfiles
![openbox](https://raw.githubusercontent.com/addy-dclxvi/dotfiles/)
<br />

## Details
### Raspberry Pi 5
- **Distro** RaspiOS (Bookworm)
- **Display Server** X11
- **Display Manager** LightDM
- **Greeter** slick-greeter
- **WM** Openbox
- **Desktop Environment** None
- **Launcher** Rofi
- **Terminal** Alacritty
- **Compositor** Picom
- **GTK Theme** Arc
- **Icons** Faba
- **Cursor** Breeze
- **Panel** polybar
- **Start Menu** personalized
- **File Manager** Thunar
- **System Tray** Trayer
- **Archiver** XArchiver
- **Video Player** MPV
- **Web Browser** Firefox ESR
- **Encoder/Decoder** ffmpeg
- **Task Manager** HTOP
- **Image Viewer** Viewnior
- **Sound Mixer** PulseAudio
- **Policy Kit Frontend** Gnome Polkit
- **Pager** Less
- **Notification Daemon** Dunst
- **CLI Shell** bash
- **CLI File Manager** Ranger
- **CLI Image Viewer** Caca
- **CLI Text Editor** nano
- **GUI Text Editor** VS Code
- **Screenshooter** scrot
- **Wallpaper Handler** Hsetroot
- **Music Player** Audacious

## How to Setup
- Install RaspiOS minimal, without any DE
- Connect to the internet
- Install git
- **Clone this repo** `git clone --depth=1 https://github.com/ ~/dotfiles` **Create github project**
- Deploy the dotfiles `cp -a ~/dotfiles/.config/. ~/.config`
- Deploy the system files `cp -a ~/dotfiles/etc/ /etc`
- Setup Openbox packages `sh ~/.scripts/openboxpack`
- Add user to sudoers using `visudo`
- Reboot
- Fix some errors
- Start working

## Keybinds & Mousebinds
### Both Openbox & Fluxbox Are Same
- **Super + Enter** launch Alacritty
- **Super + D** launch Rofi with wrapper script
- **Super + Space** launch root menu (like right click on the desktop)
- **Alt + Tab** switch to next window
- **Alt + Shift + Tab** switch to previous window
- **Control + Alt + Left/Right** switch to previous/next workspace
- **Control + Alt + Up/Down**  switch to previous/next window, just like Alt + Tab
- **Super + Arrows** "Aero Snap"
- **Super + 1-4** switch to workspace 1-4
- **Super + Shift + 1-4** take the current active window to workspace 1-4
- **Super + Shift + Left/Right** take the current active window to prev/next workspace
- **Super + Alt + Arrows** switch focus to other window in the desired direction
- **Super + Control + Arrows** teleport
- **Super + A** central the current focus window
- **Super + C** close
- **Super + Z** minimize
- **Super + F** maximize
- **Super + T** toggle the window decoration
- **Super + U** roll up the window
- **Super + Shift + Backspace** reload, do this after modify the configuration files
- **Double Click Titlebar** maximize
- **Scroll Up Titlebar** roll up window
- **Scroll Down Titlebar** restore rolled up window
- **Double Click Desktop** list opened programs, so I could survive without a taskbar (Openbox only)
- **Scrol Up/Down on Volume (Panel)** turn up/down the volume
- ..More keybinds just read the *~/.config/openbox/rc.xml* file

### Mouse Action on polybar 
- **TBD**

## Debian packages added by openboxpack script:
- arc-theme
- audacious
- breeze-cursor-theme
- ca-certificates
- caca-utils
- dosfstools
- dunst
- exiv2
- faba-icon-theme
- ffmpeg
- file
- fonts-liberation2
- gtk2-engines-pixbuf
- gucharmap
- gvfs
- gvfs-backends
- gzip
- highlight
- hsetroot
- htop
- less
- libmtp-common
- libmtp-runtime 
- libnotify-bin
- lightdm
- lightdm-gtk-greeter-settings
- mpv
- mtp-tools
- ntfs-3g
- openbox
- obconf
- p7zip-full
- pavucontrol
- policykit-1-gnome
- pulseaudio
- ranger
- rofi
- scrot
- slick-greeter
- trayer
- viewnior
- wget
- x11-xserver-utils
- xarchiver
- xdg-user-dirs
- xdg-utils
- xsel
- xserver-xorg-core
- xserver-xorg-input-kbd
- xserver-xorg-input-libinput
- xserver-xorg-input-mouse
- xsettingsd
- youtube-dl

## Notes
- If you want to use this configuration, inspect the code before use.
- If you find "addy" in the configuration file, replace it with your own username.
