# Rycroft Group meta repository
This Git repository contains code developed by the Rycroft Group at the
University of Wisconsin–Madison. The bulk of the code is provided within
submodules.

# Setting up a common configuration files
Most of the code is written in C++ and is compiled using
[GNU Make](https://www.gnu.org/software/make/). It has been tested on Linux,
MacOS, and Windows (via the WSL). The following documentation assumes you are
familiar with the Linux/Mac/WSL
[command-line interface](https://en.wikipedia.org/wiki/Command-line_interface).

To compile the code it is necessary to create a common configuration file
called **config.mk** in the parent directory, which can be used by all
subdirectories. Several templates are provided in the **config** directory. To
use, copy one of the templates into the parent directory. From the tgmr
directory, on a Linux computer, type
```Shell
cp config/config.mk.linux ../config.mk
```
On a Mac using GCC 14 installed via [MacPorts](http://www.macports.org), type
```Shell
cp config/config.mk.mac_mp ../config.mk
```
On a Mac using GCC installed via [Homebrew](http://brew.sh), type
```Shell
cp config/config.mk.mac_hb ../config.mk
```
