### global mingw64 installer 
[![global Build](https://github.com/lsq/global-mingw64-installer/actions/workflows/global-build.yml/badge.svg)](https://github.com/lsq/global-mingw64-installer/actions/workflows/global-build.yml)

- global-9.x.x_x64.zip
- mingw-w64-ucrt-x86_64-global*.pkg.tar.xz

#### install
for protable:

```bash
unzip global-9.x.x_x64.zip
```

for ucrt64:
##### Repo Installation

Add the following code snippet to your `/etc/pacman.conf`:

```conf
[lsq]
SigLevel = Optional
Server = https://github.com/lsq/global/releases/latest/download
```
Then, run `sudo pacman -Sy` to update repository.

#### Packages

##### List repo packages

```bash
pacman -Sl lsq
```

##### Install repo packages

```bash
sudo pacman -S lsq/<package-name>
```

e.g.
```bash
sudo pacman -S lsq/global
```
