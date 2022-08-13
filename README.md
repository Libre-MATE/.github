Screensaver
===========

Only [XScreenSaver](https://www.jwz.org/xscreensaver/) is supported. [mate-screensaver](https://github.com/mate-desktop/mate-screensaver) support was dropped after copyright infringements on August 10, 2022.

On Fedora you must uninstall mate-screensaver and enable xscreensaver daemon:

```
$ sudo dnf remove mate-screensaver
$ sudo sed -i '/mate-screensaver/d' /usr/libexec/xscreensaver-autostart
$ sudo sed -i '/OnlyShowIn/d' /etc/xdg/autostart/xscreensaver-autostart.desktop
```
