# yunohost-debootstrap
This script allow you to create yunohost installation with debootstrap.

## Setup on debian

```
sudo apt install debootstrap
git clone https://github.com/YunoHost/yunohost-debootstrap
sudo cp yunohost-debootstrap/yunohost /usr/share/debootstrap/scripts/
```

## Test it
```
mkdir ynh_chroot
debootstrap --include="acpi-support-base,kbd,udev,linux-image-amd64,openssh-server,ca-certificates,debhelper" yunohost ./ynh_chroot/ https://deb.debian.org/debian/
```

