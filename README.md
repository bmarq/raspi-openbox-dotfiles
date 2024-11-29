# bmarq's raspi-openbox-dotfiles
## Preview
https://github.com/bmarq/raspi-openbox-dotfiles/
<br />

### Based on addy's debian-openbox-fluxbox-dotfiles
https://github.com/addy-dclxvi/dotfiles/
<br />

## Details
### Raspberry Pi 5
- **Distro:** Raspberry Pi OS (Bookworm)
- **Display Server:** X11
- **Display Manager:** LightDM
- **Greeter:** slick-greeter
- **WM:** Openbox 3
- **Desktop Environmen:t** None
- **Launcher:** Rofi
- **Terminal:** Alacritty
- **Compositor:** Picom
- **GTK Theme:** Arc
- **Icons:** Faba
- **Cursor:** Breeze
- **Panel:** Polybar
- **Start Menu:** personalized
- **File Manager:** Thunar
- **System Tray:** Trayer
- **Archiver:** XArchiver
- **Video Player:** MPV
- **Web Browser:** Firefox ESR
- **Encoder/Decoder:** ffmpeg
- **Task Manager:** HTOP
- **Image Viewer:** Viewnior
- **Sound Mixer:** PulseAudio
- **Policy Kit Frontend:** Gnome Polkit
- **Pager:** Less
- **Notification Daemon:** Dunst
- **CLI Shell:** Bash
- **CLI File Manager:** Ranger
- **CLI Image Viewer:** Caca
- **CLI Text Editor:** nano
- **GUI Text Editor:** VS Code
- **Screenshooter** scrot
- **Wallpaper Handler:** Hsetroot
- **Music Player:** Audacious

## How to Setup:
- Install RaspiOS minimal without any DE
- Connect to the internet
- your raspi-config configuration
- Install: git openbox lightdm
- **Clone this repo** `git clone https://github.com/bmarq/raspi-openbox-dotfiles.git ~/dotfiles`
- Deploy the dotfiles `cp -a ~/dotfiles/config/. ~/.config`
- Deploy the system files `sudo cp -a ~/dotfiles/system/etc/ /etc`
- Setup Openbox packages `sudo sh ~/.config/scripts/openboxpack`
- Add user to sudoers using `visudo`
- Reboot
- Fix some errors
- Start working

## Keybinds & Mousebinds
### Openbox
- **Super + Enter** launch Alacritty
- **Super + D** launch Rofi with wrapper script
- **Super + Space** launch root menu (like right-click on the desktop)
- **Alt + Tab** switch to next window
- **Alt + Shift + Tab** switch to previous window
- **Control + Alt + Left/Right** switch to previous/next workspace
- **Control + Alt + Up/Down**  switch to previous/next window, just like Alt + Tab
- **Super + Arrows** "Aero Snap"
- **Super + 1-4** switch to workspace 1-4
- **Super + Shift + 1-4** take the current active window to workspace 1-...-n
- **Super + Shift + Left/Right** take the current active window to prev/next workspace
- **Super + Alt + Arrows** switch focus to another window in the desired direction
- **Super + Control + Arrows** teleport
- **Super + A** central the current focus window
- **Super + C** close
- **Super + Z** minimize
- **Super + F** maximize
- **Super + T** toggle the window decoration
- **Super + U** roll up the window
- **Super + Shift + Backspace** reload. Do this after modifying the configuration files
- **Double Click Titlebar** maximize
- **Scroll Up Titlebar** roll up window
- **Scroll Down Titlebar** restore rolled up window
- **Double Click Desktop** list opened programs, so I could survive without a taskbar (Openbox only)
- **Scroll Up/Down on Volume (Panel)** turn up/down the volume
- ... more keybinds just read the *~/.config/openbox/rc.xml* file

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
- firefox-esr
- fonts-liberation2
- gpm
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
- rpd-plym-splash
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
- xinit
- xsel
- xserver-xorg-core
- xserver-xorg-input-kbd
- xserver-xorg-input-libinput
- xserver-xorg-input-mouse
- xsettingsd
- youtube-dl / yt-dlp

## Notes
- If you want to use this configuration, inspect the code before use.
- If you find "bmarq" in the configuration file, replace it with your username.
