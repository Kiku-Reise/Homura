<p align="center">
  <img src="https://codeberg.org/Alexander88207/Homura/raw/branch/main/media/Banner.jpeg">
</p>

<p align="center">
	<a href="https://codeberg.org/Alexander88207/Homura/wiki/Status">Status</a>&nbsp;&nbsp;&nbsp;
	<a href="https://codeberg.org/Alexander88207/Homura/src/branch/library">Library</a>&nbsp;&nbsp;&nbsp;
	<a href="https://codeberg.org/Alexander88207/Homura/wiki/Tweaks">Tweaks</a>&nbsp;&nbsp;&nbsp;
	<a href="https://codeberg.org/Alexander88207/Homura/wiki/Borked">Borked</a>&nbsp;&nbsp;&nbsp;
	<a href="https://codeberg.org/Alexander88207/Homura/wiki/Working-Games">Working Games</a>&nbsp;&nbsp;&nbsp;
	<a href="https://codeberg.org/Alexander88207/Homura/wiki/Handbook">Handbook</a>&nbsp;&nbsp;&nbsp;
	<a href="https://codeberg.org/Alexander88207/Homura/wiki/Hints">Hints</a>&nbsp;&nbsp;&nbsp;
	<a href="https://codeberg.org/Alexander88207/Homura/wiki/Contributing">Contributing</a>
</p>

# Introduction :microphone:

Back when i started using FreeBSD, there was no useful utility to setup games or launcher in wine, so i created one myself.

Homura was developed from pure fun, so please do not take it too seriously.

Homura was created with some inspiration from lutris, but is not meant to be a substitute.

# Description &#x1F4D8;

Homura is a launcher that makes it easy to run Windows games/launcher easily on FreeBSD by providing/applying the requiered fixes and workarounds.

- The Windows emulation is provided by [Wine](https://www.winehq.org).
- The launcher menus are provided by [Zenity](https://help.gnome.org/users/zenity/)
- The most fixes that gets applied are provided by [Winetricks](https://github.com/Winetricks/winetricks)

Special thanks go to the above mentioned projects :)

# Run dependencies :syringe:

Hardware:
- A x86 CPU with 1,4 GHz or better
- A GPU with OpenGL 3.0 & 128MB VRAM or better

Software: 
- [shells/bash](https://www.freshports.org/shells/bash)
- [archivers/p7zip](https://www.freshports.org/archivers/p7zip/)
- [x11/zenity](https://www.freshports.org/x11/zenity)
- [devel/xdg-utils](https://www.freshports.org/devel/xdg-utils)
- [x11-fonts/webfonts](https://www.freshports.org/x11-fonts/webfonts)
- [emulators/winetricks](https://www.freshports.org/emulators/winetricks)
- [devel/vulkan-tools](https://www.freshports.org/devel/vulkan-tools)
- [graphics/mesa-demos](https://www.freshports.org/graphics/mesa-demos)
- [x11-fonts/noto-extra](https://www.freshports.org/x11-fonts/noto-extra) (Optional)
- [x11/antimicro](https://www.freshports.org/x11/antimicro) ([Optional](https://gitlab.com/Alexander88207/Homura/-/wikis/Controllers#guitar-hero-world-tour-guitar-pc-guitar-hero-3-guitar-les-paul-ps3))
- [emulators/i386-wine-devel](https://www.freshports.org/emulators/i386-wine-devel) on amd64 or [emulators/wine-devel](https://www.freshports.org/emulators/wine-devel) on i386

# Installation/Uninstallation :cd:

### Installing from FreeBSD repository 📦

Note: Packages can lag behind ports. If you want the latest version you may want to use the `latest` repository instead of `quarterly` or build the package yourself.

`# pkg install games/homura`

### Build & installing the port from FreeBSD ports collection ⚙️

`cd /usr/ports/games/homura/ && make install clean`

### Installing from source ⚙️

Please only do this, if you know what are you doing.

```
cd /usr/local/bin
fetch https://codeberg.org/Alexander88207/Homura/raw/branch/main/Homura
chmod +x Homura
```

### Uninstallation

`# pkg uninstall games/homura`

To also delete the related games etc...

Use the "Delete and reset everything" function.

# Usage :computer:

Homura was created for the gui usage in the first place, the gui can be opened via the commandline `Homura` but also via a shortcut (if you have Homura allowed to create one).

For terminal fans there are also some fast commands:

Examples: 

- To install something use `Homura Install  Steam`
- To launch something use `Homura Launch Steam`
- To uninstall something use `Homura Uninstall Steam`

# Feature / Extra / To-Do list

Features | Done?
------------ | -------------
Installation launching & uninstallation of our collection of applications (Main features) | :heavy_check_mark:
Custom prefixes | :heavy_check_mark:
Shortcut creation | :heavy_check_mark:
Delete & reset everything | :heavy_check_mark:
Enable/Disable DXVK | :heavy_multiplication_x:
Tinkering | :heavy_check_mark:
Changing between wine versions | ⌛

# Limitations :x:

- Only 32-Bit Games and Applications working currently because of current situation how wine gets shipped from ports.
- No winevulkan for 32bit Wine on amd64. Reason: The package dont contains the lib32 vulkan library.

# Chat :speech_balloon:

You need fast help, want to help or just want to talk?  ／人◕ ‿‿ ◕人＼ 

- Join our [Discord](https://discord.gg/JBKcdNt)
- Join the [GhostBSD Telegram Group](https://t.me/ghostbsd)
- Contact the Maintainer on [Steam](https://steamcommunity.com/id/Alexander88207)


# Credits :star:

- [Alexander88207](https://codeberg.org/Alexander88207) - Lead programmer & Maintainer
- [Epychan](https://steamcommunity.com/profiles/76561198055067377) - Testing games and reporting fixes
- [Brandon Ayers](https://github.com/thedaemon) - Testing games
- [MagZu](https://github.com/magzu) - Hosting the mirror (homura.magzu.net)
- [You?](https://codeberg.org/Alexander88207/Homura/wiki/Contributing)

# Screenshots

![](https://codeberg.org/Alexander88207/Homura/raw/branch/main/media/Screenshot.png "Screenshot")

![](https://codeberg.org/Alexander88207/Homura/raw/branch/main/media/Screenshot4.png "Screenshot")

<img src="https://codeberg.org/Alexander88207/Homura/raw/branch/main/media/Screenshot2.png" alt="Monitor" height="500" width="700"> 

<img src="https://codeberg.org/Alexander88207/Homura/raw/branch/main/media/Screenshot3.png" alt="Monitor" height="500" width="700"> 

# Videos

Preview: https://www.youtube.com/watch?v=6B1h0F4rIs4

- Review by RoboNuggie: https://www.youtube.com/watch?v=0lLs3JxezBM
- Review by Linux Lounge: https://www.youtube.com/watch?v=BLNuRwLm2FI
- BSD-PL November 2019: https://www.youtube.com/watch?v=X68aGybmHwI&t=2029s

- A whole channel who is sharing the expierence: https://www.youtube.com/channel/UCDQRT3fw3n1XiAygboszP1A