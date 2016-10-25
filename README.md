## My rEFInd theme

This repository represents my current bootloader theme.

![initramfs' rEFInd theme](https://i.imgur.com/8ddmLhT.png)

## Usage

1. Copy the themes folder from this repository into your rEFInd directory within your EFI partition.
2. Copy the initramfs-theme.conf to your rEFInd directory within your EFI partition.
3. Edit your refind.conf file to include the initramfs-theme.conf file.
4. For Windows, Arch Linux or Gentoo Linux systems, point the icon to EFI/refind/themes/initramfs/icons/os_win.png, EFI/refind/themes/initramfs/icons/os_arch.png or EFI/refind/themes/initramfs/icons/os_gentoo.png respectively.

Since rEFInd has no mechanism for a primary title, the title has been baked into the banner (background) file. A PSD file is provided containing both the raw background and the foreground title as seperate layers such that you can generate your own banner.png from that.
Replace the file in themes/initramfs/banner.png

Given that I have a 4K panel, some of these graphics may be extremely large on lower resolution screens. In those cases, halving the resolution of the icons (and setting the new sizes as appropriate in the initramfs-theme.conf file) can be done for proper scaling. Note: I haven't tweaked any resolution settings in rEFInd, my system seems to automatically load a full resolution bootloader (some systems run reduced-resolution bootloaders). 

## Attribution

This theme was inspired by [rEFInd-minimal](https://github.com/EvanPurkhiser/rEFInd-minimal/) in terms of style.

The arch icon was taken directly from the [Arch Linux website](https://www.archlinux.org/art/), whereas the rest I simply found via google image search and modified them to fit my scheme.
Since this was initially merely a private project, I apologize for not providing sources to where I got the images (I don't really remember anymore). 
