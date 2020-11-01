# Minipro - Chocolatey Package

This repo contains the choco package artefacts for installing the [Minipro universal programmer](https://gitlab.com/DavidGriffith/minipro/) on your Windows machine.

The original repo was compiled using [Cygwin](https://www.cygwin.com/) which means that `minipro.exe` needs to be distributed with `cygwin1.dll` in order to run on Windows.

> **IMPORTANT:** This package isn't as streamlined as I would like it to be. `minipro.exe` currently requires the `infoic.xml` file to be in the `current working directory` in order to be able to select supported devices. Therefore, if you install this package, make sure you have `infoic.xml` located in the directory you will be running the `minipro` command from. The [infoic.xml can be found here](https://github.com/bberak/minipro-choco/blob/master/tools/infoic.xml).

## Prerequisites

- [Chocolatey](https://chocolatey.org/)

## Installing Package

Build the .nupkg:

```
git clone https://github.com/bberak/minipro-choco.git
cd minipro-choco
choco pack
```

Intall the .nupkg using choco:

```
choco install minipro -s "."
```

You can now run minipro from the commandline:

```
minipro
```

## Uninstalling Package

To remove, simply run:

```
choco uninstall minipro
```
