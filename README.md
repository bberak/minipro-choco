# Minipro - Chocolatey Package

This repo contains the choco package artefacts for installing the [Minipro universal programmer](https://gitlab.com/DavidGriffith/minipro/) on your Windows machine.

The original repo was compiled using [Cygwin](https://www.cygwin.com/) which means that `minipro.exe` needs to be distributed with `cygwin1.dll` in order to run on Windows.

## Prequisites

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
choco install minipro -s ".\"
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