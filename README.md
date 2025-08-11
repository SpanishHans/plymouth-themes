<h1 align="center">Plymouth Themes</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Maintained%3F-Yes-green?style=for-the-badge">
  <img src="https://img.shields.io/github/license/SpanishHans/plymouth-themes?style=for-the-badge">
  <img src="https://img.shields.io/github/stars/SpanishHans/plymouth-themes?style=for-the-badge">
  <img src="https://img.shields.io/github/forks/SpanishHans/plymouth-themes?color=teal&style=for-the-badge">
  <img src="https://img.shields.io/github/issues/SpanishHans/plymouth-themes?color=violet&style=for-the-badge">
</p>

<p align="center">
A big collection of plymouth themes, ported from <i>android bootanimation</i> from <a href="https://forum.xda-developers.com/android/themes/alienware-t3721978">here.</a>
</p>

![gif](https://raw.githubusercontent.com/SpanishHans/plymouth-themes/main/previews/rango.gif)

### What is plymouth?

[Plymouth](http://www.freedesktop.org/wiki/Software/Plymouth) is a project from Fedora and now listed among the [freedesktop.org's official resources](https://www.freedesktop.org/wiki/Software/#graphicsdriverswindowsystemsandsupportinglibraries) providing a flicker-free graphical boot process. It relies on [kernel mode setting](https://wiki.archlinux.org/index.php/Kernel_mode_setting) (KMS) to set the native resolution of the display as early as possible, then provides an eye-candy splash screen leading all the way up to the login manager.

### How to get set up?

follow [this](https://wiki.archlinux.org/index.php/plymouth) *archwiki* article to setup plymouth in *archlinux* or any other distro.

### Arch user?
> If you `Use arch BTW`, you are in luck because the themes are in the AUR as 
```bash
paru -S plymouth-theme-THEME-git
```

### How to get these themes in you are a peasant?

1. **Get themes:** Get whatever theme you want from this repo however you want.

	- **Download** individual themes from [**releases**](https://github.com/SpanishHans/plymouth-themes/releases).
	- **Clone** this repo with `git clone https://github.com/SpanishHans/plymouth-themes.git`
	- **Wget** the files with an overcomplicated script by yourself.

2. **Copy to plymouth dir:** place the theme's dir in `/usr/share/plymouth/themes`. 
```bash
tar -xvf THEME.tar.gz # or whatever the cool kids use.
cp -r THEME /usr/share/plymouth/themes
ls /usr/share/plymouth/themes
```

3. **Check install:** Themes must be recognized by plymouth by running the following command if all the above was done correctly.
```bash
sudo plymouth-set-default-theme -l
```

4. **Set theme** Set the plymouth theme to the selected theme by running the following command.
```bash
sudo plymouth-set-default-theme -R THEME
```

### Previews

<!----------------------------- Pack 1 ----------------------------->
<details><summary>Pack 1</summary>

| Name | Preview |
|-------|---------|
| rango | ![gif](https://raw.githubusercontent.com/SpanishHans/plymouth-themes/main/previews/rango.gif) |

+ [Rango](https://raw.githubusercontent.com/SpanishHans/plymouth-themes/main/previews/rango.gif)
</details>

### FYI
+ Created and tested on machine with 2560x1440 resolution.
+ initramfs becomes big, therefore slower boot.
+ Sometimes for machines with very fast boot with other DM different than `Gdm`, an special delay is needed. READ THE WIKI.
