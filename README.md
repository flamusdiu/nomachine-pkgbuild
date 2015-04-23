Simple PKGBUILD to install nomachine NX

>**Clone NoMachine NX**
```
git clone git@github.com:ElectricPrism/nomachine-pkgbuild.git
```

_Enter NoMachine NX Directory
```
cd ~/nomachine-pkgbuild
```

_Make the Package
```
makepkg -s
```

_Merge The Package Into The System
```
sudo pacman -U nomachine-4.5.0-1-x86_64.pkg.tar.xz
```
