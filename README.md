# mcc-build

Builds a linux package out of the mcc source

## PREREQUISITES

1. Install git
2. If not already installed, install base-devel for makepkg

## BUILD INSTRUCTIONS

1. Copy paste these following commands into any terminal

```bash
cd /tmp
git clone https://github.com/Mediocre-Games-United/mcc-build.git
cd mcc-build
makepkg -si
rm -rf /tmp/mcc-build
```

