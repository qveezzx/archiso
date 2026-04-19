# ZuccOS

ZuccOS is a minimalist, performance-focused Arch Linux distribution. It’s designed to be fast on high-end PCs while remaining lightweight enough to run perfectly on older hardware. 

The goal is a clean base that stays out of your way and gives you the performance Arch is known for, but with better defaults for modern hardware.

## Core Features

- **CachyOS RT-BORE Kernel**: Replaced the standard kernel with `linux-cachyos-rt-bore`. It uses the BORE scheduler and real-time optimizations for better responsiveness and lower latency.
- **Openbox Desktop**: Using Openbox because it’s incredibly light and stays out of the way of your system resources.
- **systemd-boot**: Moved away from GRUB2 in favor of `systemd-boot`. It’s faster, simpler, and much more modern for UEFI systems.
- **Custom systemd Setup**: Includes a custom systemd service.
- **Calamares Installer**: Includes the Calamares graphical installer so you can get the system onto your drive without manual partitioning or terminal setup.
- **Automated Builds**: Every ISO is built automatically using GitHub Actions and pushed to the releases page.

## Installation

1. Grab the latest `.iso` from the [Releases](https://github.com/qveezzx/archiso/releases/latest) page.
2. Flash it to a USB drive (2GB or larger) using `dd`, Ventoy, or Etcher/Rufus.
3. Boot into the live environment and launch the installer from the desktop.

## Note on Stability
This is a rolling release project. Builds are automated and not manually tested before they go live. If you're planning to install this, it's a good idea to check the `build.log` in the latest release to make sure everything finished correctly.

---
Built with Archiso. Base: Arch Linux.
