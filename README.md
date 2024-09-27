# Welcome to the .dotfiles of my Archlinux Gruvbox themed Sway setup

After using a combination of various other dotfiles from generous people on Github, combined with my own adjustments, I decided to share my current setup too. Also, many thanks to the kind internetstrangers at <A HREF="https://www.reddit.com/r/unixporn/">r/unixporn</A> for their wonderful creations.
I'm running Archlinux with Sway as my window manager. I used the "gruvbox" colors as much as possible.  Rofi is used as an application launcher.

This repository contains my dotfiles in a .tar file which you can extract to your ~/.config folder.

I also added a file called packages.txt containing all the packages I currently have installed.  If I ever break my system it can be a useful list to have.

# Important keyboard shortcuts
> $mod = Mod4 (Windows key)
> 
> $mod+d = rofi
> 
> $mod+Enter = foot
> 
> $mod+t = Thunar
> 
> $mod+m = g4music
> 
> $mod+q = kill
> 
> $mod+r = resize
> 
> $mod+v = split vertically
> 
> $mod+b = split horizontally

Because I use an AZERTY keyboard layout I had to use 'wev' to find out how keypresses are handled.  That's why you will see lines like ```bindsym $mod+ampersand workspace number 1``` and ```bindsym $mod+eacute workspace number 2``` etc in the .config/sway/config file.


# Show me!
Clean:
![Clean desktop.](https://github.com/himselfish/dotfiles/blob/main/desktop_clean.png)

Busy:
![Busy desktop.](https://github.com/himselfish/dotfiles/blob/main/desktop_fake_busy.png)

Rofi:
![Rofi](https://github.com/himselfish/dotfiles/blob/main/desktop_rofi.png)
