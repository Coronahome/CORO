
Debian
====================
This directory contains files used to package coronaathomed/coronaathome-qt
for Debian-based Linux systems. If you compile coronaathomed/coronaathome-qt yourself, there are some useful files here.

## coronaathome: URI support ##


coronaathome-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install coronaathome-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your coronaathomeqt binary to `/usr/bin`
and the `../../share/pixmaps/coronaathome128.png` to `/usr/share/pixmaps`

coronaathome-qt.protocol (KDE)

