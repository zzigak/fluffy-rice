# Fluffy rice
## Follow this guide to get the exact same rice as mine.
### Time required: ~ 30 min


# 1. Base installation

The base OS for this setup will be installed using Endeavour OS calamares installer. You should opt for the minimal (vanilla) install with minor additions that will be mentioned now.

To get the exact results make sure to check the following packages/options in the installer:

//2 screenshots

additionaly you should select one of the terminals which come prepackaged with other desktop environments (e.g. konsole, gnome terminal...). I use the xfce4-terminal.

After the installation has finished reboot the system and remove the installation medium. 
At this point you (should) have a minimal arch install on your system.

# 2. Installing WM, DM and basic packages

Now we will install the basic packages we will need to "cook" our rice the "right" way.

Firt the best WM, claerly being AwesomeWM, will be installed:

```
sudo pacman -S awesome
```

Then you should go forth and install your DM (display manager) of your choice. In my case the minimal, lightweight DM, ly:

```
yay -S ly
```

Before the end of this section we should install packages that'll equip our setup with all the needed programs. For me, this are the following packages:



| Type | Name |
|: ---: |: ---: |
|Browser | Firefox |
|Terminal  |Alacritty|
| Text editor & IDE | NeoVim & Visual Studio Code  |
| Wallpaper setter |Nitrogen  |
|Fetch  |pfetch  |
| Video player |mpv  |
|  Conferencing| Zoom |
| Transparency (not used) | picom |
| File manager | Thunar & ranger |
| Screenshots | Flameshot |
| Screen capture |OBS  |
| Customisation | lxappearance |
| GTK & Icon theme |dracula-gtk-theme papirus-icon-theme  |
| PDF/file reader|Zathura & zathura-pdf-mupdf   |
| Communication |Discord & Whatsapp & Slack  |

These packages can be installed all at once with the following 2 commands:

```
sudo pacman -S firefox nitrogen alacritty neovim mpv zoom picom thunar ranger flameshot lxappearance dracula-gtk-theme papirus-icon-theme zathura zathura-pdf-mupdf discord slack

yay -S pfetch visual-studio-code-bin whatsapp-for-linux slack-desktop 

```

Lastly, to setup the WM you must add the following line to your .xinitrc file as follows:

```
echo "exec awesome" > ~/.xinitrc"
```

To enter awesome run the following command:

```
startx
```


# 3. Customisation


