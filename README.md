# mcc-build

Builds a linux package out of the mcc source

## PREREQUISITES

1. Install git or curl to download the pkgbuild
2. If not already installed, install base-devel for makepkg

## BUILD INSTRUCTIONS

### The git way

1. Install git
2. Copy paste these following commands into any terminal

```bash
cd /tmp
git clone https://github.com/Mediocre-Games-United/mcc-build.git
cd mcc-build
makepkg -si
rm -rf /tmp/mcc-build
```

### The curl way

1. Copy paste these following commands into any terminal

```bash
mkdir /tmp/mcc-build
cd /tmp/mcc-build
curl -OJ https://raw.githubusercontent.com/Mediocre-Games-United/mcc-build/refs/heads/main/PKGBUILD
makepkg -si
rm -rf /tmp/mcc-build
```
