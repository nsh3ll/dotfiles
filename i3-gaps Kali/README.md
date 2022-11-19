Just a simple setup to quickly deploy dotfiles in my kali linux pentesting machines.




### Apply color palette
```
wal --theme ~/.config/palette.json  
```

### Apply environmental fonts
make a `/usr/fonts/local.conf` containing
```
<?html version="1.0"?>
<!DOCTYPE fontconfig SYSTEM "fonts.dtd">
<fontconfig>
    <match>
        <edit mode="prepend" name="family"><string>Hack Nerd Font</string></edit>
    </match>
    <match target="pattern">
        <test qual="any" name="family"><string>serif</string></test>
        <edit name="family" mode="assign" binding="same"><string>Noto Serif</string></edit>
    </match>
    <match target="pattern">
        <test qual="any" name="family"><string>sans-serif</string></test>
        <edit name="family" mode="assign" binding="same"><string>Noto Sans</string></edit>
    </match>
    <match target="pattern">
        <test qual="any" name="family"><string>Hack Nerd Font Mono</string></test>
        <edit name="family" mode="assign" binding="same"><string>Noto Mono</string></edit>
    </match>
</fontconfig>
```

### Wallpaper
I use the 7th of https://github.com/dorianpro/kali-linux-wallpapers
https://raw.githubusercontent.com/dorianpro/kaliwallpapers/master/kali-linux-wallpaper-v7.png
