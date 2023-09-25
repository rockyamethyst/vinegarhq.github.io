# Installation from Flatpak

Vinegar's Flatpak can be found [here](https://flathub.org/apps/details/io.github.vinegarhq.Vinegar). 

Installing it manually from a terminal:
```
flatpak install flathub io.github.vinegarhq.Vinegar
flatpak run io.github.vinegarhq.Vinegar
```



# Building Flatpak from source

**Note**: Vinegar's Flatpak comes with it's own Wine build-system, so be prepared to compile Wine.

To build Vinegar, you will need `flatpak-builder` installed on your system.

Clone Vinegar's Flatpak git repository manifests and build the Flatpak:
```
git clone https://github.com/vinegarhq/io.github.vinegarhq.Vinegar
cd io.github.vinegarhq.Vinegar
make
```

If you see errors about missing runtimes, make sure to install those with `flatpak install --user <runtime>`.

# Uninstalling from flatpak
To uninstall Vinegar from a terminal:
```
flatpak uninstall --delete-data io.github.vinegarhq.Vinegar
``` 
