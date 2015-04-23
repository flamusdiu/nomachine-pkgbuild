Simple PKGBUILD to install nomachine NX

1. **Clone NoMachine NX**
```
git clone git@github.com:ElectricPrism/nomachine-pkgbuild.git
```

2. **Enter NoMachine NX Directory**
```
cd ~/nomachine-pkgbuild
```

3. **Make the Package**
```
makepkg -s
```

4. **Merge The Package Into The System**
```
sudo pacman -U nomachine-4.5.0-1-x86_64.pkg.tar.xz
```
