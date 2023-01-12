# manjaro-iso-profiles
Manjaro iso Images for Juno Tablet

## Manjaro
The iso needs to be built on top of Manjaro, make sure you have kernel 6.1 or higher installed on your machine.

## Install Manjaro Tools
```sudo pacman -S manjaro-tools-iso git```

## Download the latest ISO profiles
```git clone https://github.com/junocomp/manjaro-iso-profiles.git ~/iso-profiles```

```cd manjaro-iso-profiles```

## Prepare manjaro-tools.conf
```mkdir -p ~/.config/manjaro-tools```

```cp manjaro-tools.conf ~/.config/manjaro-tools```

## ISO Images
```cutefish```

```plasma-bigscreen```

```plasma-mobile```

## Build ISO
Make sure to replace ```isoimage``` from one of the list above

```buildiso -p isoimage```

When the build process finishes successfully, the ISO file and the package list will appear in this folder:

```/var/cache/manjaro-tools/iso/```

## More info
https://wiki.manjaro.org/index.php/Build_Manjaro_ISOs_with_buildiso
