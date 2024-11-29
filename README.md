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
- **Desktop Environment:** None
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
- Install: git openbox lightdm slick-greeter
- create file /etc/lightdm/slick-greeter.conf with:\
[Greeter]\
draw-grid=false\
background=/usr/share/images/desktop-base/default (or other)

- **Clone this repo** `git clone https://github.com/bmarq/raspi-openbox-dotfiles.git ~/dotfiles`
- Deploy the dotfiles:\
  `cp -a ~/dotfiles/config/. ~/.config`\
  `cp -a ~/dotfiles/config/fontconfig ~/.fontconfig` \
  `cp -a ~/dotfiles/config/themes ~/.themes`\
  `cp -a ~/dotfiles/config/scripts ~/.scripts`
- Deploy the system files `sudo cp -a ~/dotfiles/system/etc/ /etc`
- Setup Openbox packages `sudo sh ~/.scripts/openboxpack`
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
- blueman
- breeze-cursor-theme
- ca-certificates
- code
- conky
- dosfstools
- dunst
- faba-icon-theme
- ffmpeg
- file
- firefox-esr
- fonts-liberation2
- gzip
- highlight
- hsetroot
- htop
- less
- libmtp-common
- libmtp-runtime
- libnotify-bin
- man-db
- mpv
- mtp-tools
- ntfs-3g
- p7zip-full
- pavucontrol
- picom
- policykit-1-gnome
- pulseaudio
- ranger
- rofi
- rxvt-unicode
- scrot
- tlp
- trayer
- thunar / thunar-archive-plugin
- viewnior
- wget
- xdg-user-dirs
- xdg-utils
- xsel
- xsettingsd
- youtube-dl / yt-dlp

## Notes
- If you want to use this configuration, inspect the code before use.
- If you find "bmarq" in the configuration file, replace it with your username.
