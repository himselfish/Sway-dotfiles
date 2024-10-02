# Welcome to the .dotfiles of my Archlinux Gruvbox themed Sway setup

After using a combination of various other dotfiles from generous people on Github, combined with my own adjustments, I decided to share my current setup too. Also, many thanks to the kind internetstrangers at <A HREF="https://www.reddit.com/r/unixporn/">r/unixporn</A> for their wonderful creations.<BR />
I'm running Archlinux with Sway as my window manager. I used the "gruvbox" colors as much as possible.  Rofi is used as an application launcher.<BR />
<BR />
This repository contains my dotfiles in a .tar file which you can extract to your ~/.config folder.<BR />
<BR />
I also added a file called packages.txt containing all the packages I currently have installed.  If I ever break my system it can be a useful list to have.  You probably don't need all those packages.

# Important keyboard shortcuts

| Key(s) | Description |
| --- | --- |
| $mod | Mod4 (Windows key) |
| $mod+d | Rofi |
| $mod+Enter | foot terminal |
| $mod+t | Thunar |
| $mod+m | g4music |
| $mod+c | Firefox |
| $mod+q | Kill |
| $mod+r | Resize mode (use arrow keys to resize, then press ENTER or ESC) |
| $mod+v | Split vertically |
| $mod+b | Split horizontally | 
| prtsc | Sway-interactive-screenshot |
| $mod + prtsc | Sway-interactive-screenshot --video |
| $mod+s | Layout stacking |
| $mod+e | Layout split |
| $mod+w | Layout tabbed |
| $mod+f | Full screen |
| $mod+Shift+Space | Toggle floating |

Because I use an AZERTY keyboard layout I had to use ```wev``` to find out how keypresses are handled.  That's why you will see lines like ```bindsym $mod+ampersand workspace number 1``` and ```bindsym $mod+eacute workspace number 2``` etc in the .config/sway/config file.<BR />


# Scratchpad
One of the best features of tiling window managers is scratchpad.  I'm not going to explain in details what it is but you can consider it like an invisible workspace where you can send windows to and retrieve from.  Here are the keybinds that will make your life a whole lot easier.<BR />
Move to scratchpad : ```bindsym $mod+Shift+minus move scratchpad```<BR />
Toggle between windows in scratchpad : ```bindsym $mod+minus scratchpad show```<BR />
And my absolute favorite is the Quake-style terminal : ```bindsym $mod+Ctrl+Return exec --no-startup-id "sway-scratchpad -tmt -atc foot fish"```. Pressing $mod+Ctrl+Return again will hide your terminal.  <BR />

# Automatic Timeshift backups
Timeshift is a very useful tool to automatically create backups of your device.   It can be installed from AUR (```extra/timeshift 24.06.3-1 ``` at the time of writing).  To launch it in Sway enter ```sudo -E timeshift-gtk```. <BR />
Archlinux does come with cronie installed by default, but it's not started at boot.  Enter ```sudo systemctl enable --now cronie && systemctl enable --now cronie.service```.  Timeshift will now create automatic backups based on your prferences.  This can be daily, hourly, at boot,...  Yes, I'm well aware of the pacman hooks that allow for btrfs snapshots before updating too.  I just prefer this method.<BR />

# Show me!
Clean:
![Clean desktop.](https://github.com/himselfish/dotfiles/blob/main/desktop_clean.png)

Busy:
![Busy desktop.](https://github.com/himselfish/dotfiles/blob/main/desktop_fake_busy.png)

Rofi:
![Rofi](https://github.com/himselfish/dotfiles/blob/main/desktop_rofi.png)
