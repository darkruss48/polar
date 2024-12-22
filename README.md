# Polar
A simple, powerfull WT Performance Analyser for Dragon Ball Z : Dokkan Battle.

## Installation

Check the releases.

## Build

You might want to build your own version of Polar.
To do so, you need to download it using [QT](https://qt.io).
I made this client using my own static QT build (v6.8.0) on Windows 11, which allows me to compile it and to share it without you needing to install QT.
If you build it yourself with the distribued version of QT (the dynamic one), it will work for you but you can't share your executable as it need to have QT installed on the computer to start.
Feel free to contact us (check [contact](#Contact)) if you need any help to compile it.

- If you're using Windows, just download Polar from the releases page.
- If you're using Linux, you may want to build it yourself.

### Linux

In my case, I used Arch Linux to compile Polar.
The main difference compared to other distro should be the command to install all QT packages needed.
Use your prefered package manager and download QT 6.

First, download these packages to download QT 6:
```bash
sudo pacman -S qt6 qt6-base qt6-charts
```

**:warning: A lot of display manager and desktop environment such as SDDM, KDE, LXQt, and many other use QT 5.x. If you're using one of these, you may have QT 5.x already installed on your device. We highly recommand to use QT 6.x to compile Polar.**

Polar can be built with Qt 5.x, but don’t expect the program to function as it should. Consider using QT 6.x.


Once done, clone this repo :
```bash
git clone https://github.com/darkruss48/Polar
cd Polar
```
Create the build folder and cd into :
```bash
mkdir build
cd build
```

Compile the translations file by typing this command :
```bash
/usr/lib/qt6/bin/lrelease ../*.ts
```

Finally, use qmake and make to compile Polar :
```bash
/usr/lib/qt6/bin/qmake ..
make
```
Start the client :
```bash
./Polar
```

## Contributors

This project was made possible thanks to the hard work and dedication of the following individuals:

- **Polo** : [GitHub Profile](https://github.com/polowiper)
- **Darkruss** : [GitHub Profile](https://github.com/darkruss48)

## Contact
Contact me on [Twitter](https://twitter.com/darkruss47) or reach me on discord : darkruss (or polo as well)
