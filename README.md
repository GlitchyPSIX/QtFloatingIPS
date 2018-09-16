Qt Floating IPS
================

[![Snap Status](https://build.snapcraft.io/badge/covarianttensor/QtFloatingIPS.svg)](https://build.snapcraft.io/user/covarianttensor/QtFloatingIPS)

Qt Floating IPS is a patcher for IPS and BPS files. Uses Qt5 and QML for the interface and is powered by the Floating IPS library written by Alcaro on Github.

## Libraries Used
+ [FloatingIPS](https://github.com/Alcaro/Flips) by [Alcaro](https://github.com/Alcaro). Repository [*(GPL 3.0+)*](https://raw.githubusercontent.com/Alcaro/Flips/master/COPYING.gpl3): [https://github.com/Alcaro/Flips](https://github.com/Alcaro/Flips)
---
## How to Install (on OS X)
Compiled binaries for OS X are available. Download from the releases page (link below), then unzip and just drag and drop into your Applications folder.

### OS X Releases
+ OS X binaries can be found [here](https://github.com/covarianttensor/QtFloatingIPS/releases).
---

### Building From Source
First clone the repository using `git`, if you don't have `git` installed
you can find installation instructions [here](https://git-scm.com).

However, it is **strongly recommended** that you can install `git` as part of the `Xcode Command Line Tools`,
because you will need the command line tools to use the `brew` package manager.
More information about `Xcode` can be found [here](https://developer.apple.com/xcode/).

```
$ git clone https://github.com/covarianttensor/QtFloatingIPS.git
```

Next we need to make sure we have `brew` installed for OS X. If you don't
already have `brew` installed you can find installation instructions [here](https://brew.sh/).

Now we need to install the qt5 development libraries and tools, the
command for `brew` is listed below:

```
# brew install qt
```

You should then have access to `qmake`, `make`, and the qt5 development
libraries. Next `cd` into the project folder inside the repo:

```
$ cd QtFloatingIPS/QtFloatingIPS
```

You can specify the target directory using the `PREFIX` `qmake` variable (default: `/usr/local`).
Now run `qmake`, this will auto generate a makefile:

```
$ qmake PREFIX=/usr
```

Then run `make` to build the project:

```
$ make
```

And finally run `make install` to install the app:

```
# make install
```

Now you're good to go!

## Screenshots (OS X)
![Alt text](/docs/sc1.png?raw=true "Running on OS X")

![Alt text](/docs/sc2.png?raw=true "Running on OS X")
