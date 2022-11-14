# xfce4-windowck-plugin

Xfce panel plugin which allows to put the maximized window title and windows buttons on the panel.

Original plugin's features:

* Show the title and buttons of the maximized window on the panel.
* Allow window actions on buttons and title clicks (activate, (un)maximize, close).
* Allow window action menu on left button click.
* Title formatting options.
* xfwm4/unity theming support for buttons. (xfwm4 theme support reenabled in this fork)

FAQ:  
Q: How do I hide the window decorations on maximized windows on Xfce?  
A: Xfce 4.12 now support Titileless feature! Enable it in Window manager tweaks → Accessibility.

This code is derived from original 'Window Applets' from Andrej Belcijan.
See <https://www.gnome-look.org/p/1115400> for infos.

## Screenshots

See [this page](https://goodies.xfce.org/projects/panel-plugins/xfce4-windowck-plugin) for (dated) screenshots.

## Installation

### Arch Linux

For Arch Linux users [AUR package](https://aur.archlinux.org/packages/xfce4-windowck-plugin-xfwm4-theme-support/) is available with xfwm4 theme support reenabled (built from this repo).
Or use [AUR package](https://aur.archlinux.org/packages/xfce4-windowck-plugin/) for the package built from official XFCE sources

### Other Linux distributions

* Install dependencies:
  * For Debian/Ubuntu see `debian/control` folder and follow Debian packaging guidelines
* Generate common makefiles:
  
  ```bash
  ./autogen.sh --prefix=/usr
  ```

* Compile and install the plugin:

  ```bash
  make
  sudo make install
  ```

## How to report bugs?

Bugs should be reported right to this [GitHub page](https://github.com/twa022/xfce4-windowck-plugin/issues) especially if related to the button theme.
