# qemu-git-patched-pkgbuild
[qemu-git](https://www.archlinux.org/packages/extra/x86_64/qemu/) from AUR, PKGBUILD patched for anti-vm detection.

Just replaces strings to support VM hiding.

This along with thebetter-timing kernel patch and common-sense changes to libvirt xml clears all pafish checks.

# Install
1. Clone
1. Change string values in ``PKGBUILD`` to be unique
1. Build with dependencies ``makepkg -s`` (double check /etc/makepkg.conf for parallel compilation or this will take forever)
1. Install with pacman ``pacman -U qemu-git-<version>.pkg.tar.zst``
