Full Form **CPU Schecutil Governor**. It't basically a systemd service to always switch to schedutil cpu governor on boot.

NOTE: ITS ONLY MEANT FOR INTEL CPUs.
# Installation
## Get PKGBUILD
$ ``` curl -L https://raw.githubusercontent.com/humanbeing27/plymouth-theme-arch-spinner/main/PKGBUILD -o ./PKGBUILD ```
## Build and Install
$ ``` makepkg -sircC ```
# Enabling the Service
#``` systemctl enable cpumoder ```

$``` reboot ```
