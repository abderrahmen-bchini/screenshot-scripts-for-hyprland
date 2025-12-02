# Screenshot Scripts for Hyprland (Wayland)

I made three tiny scripts using **grim** and **slurp** to take screenshots of your **window**, **screen**, or **a selected area**. Nothing fancy, just stuff that actually works.

## Requirements

You need **grim** and **slurp** installed. You can look up how to install them on your distro, but since I use Arch ( btw ), here’s mine:

```bash
sudo pacman -S grim slurp
```

The scripts are so simple that they make me wonder why *hyprshot* refused to function from day one—and why Hyprland acts allergic to binding it to my keys. anyways…

Download the files (**hs_area.sh**, **hs_screen.sh**, **hs_window.sh**) and throw them somewhere. I keep mine in `~/bin/scripts` like a civilized person.
Don’t forget to give them executable permissions:

```bash
chmod +x hs_area.sh  
chmod +x hs_screen.sh
chmod +x hs_window.sh
```

Then bind them in your `hyprland.conf`.
(Obviously, change the paths to wherever you stored your scripts.)

```
bind = SUPER, F12, exec, ~/bin/scripts/hs_screen.sh  
bind = SUPER, F11, exec, ~/bin/scripts/hs_window.sh
bind = SUPER, F10, exec, ~/bin/scripts/hs_area.sh
```

And that’s it. Hope it helps—and hey, feel free to ⭐ the repo if you like my work.
