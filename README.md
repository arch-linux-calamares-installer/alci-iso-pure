# ALCI PURE ARCH

This iso attempts to be the purest of Arch Linxu installations.

# Arch Linux Calamares Installer or ALCI

Use the correct version of Archiso to build the iso.

**Read the archiso.md.**

Download the content of the github with (use the terminal)

`git clone https://github.com/arch-linux-calamares-installer/alci-iso-pure`

# Pacman.conf in archiso folder

Only the archiso/pacman.conf will be used to download your packages.


# Pacman.conf in archiso/airootfs/etc/

This will be your future system. 
Include the repositories you want.
It will not be used to build the iso.


# Archiso/packages.x86_64

Only the archiso/packages.x86-64 files will be used.

Add more packages at the bottom of the file


# Build process


Use the scripts from this folder:

<b>installation-scripts</b>

Use script 30 and it will clean your pacman cache and redownload every package it needs.

Use script 40 to use your current pacman cache - it will only download what is needed

You will find the iso in this folder:

 ~/Alci-Iso-Pure-Out

Burn it with etcher or other tools and use it.




# Tip

Sometimes a "proc" folder stays mounted.

Unmount it with this

sudo umount /home/{username}/...  use the TAB



# Tip

Run into issues - remove all packages manually with

`sudo pacman -Scc`

and ensure they are all gone.


# Tip

When testing out the ALCI in virtualbox, you can use the alias 
evb to enable and start virtualbox. As a result you can use your full resolution.



# Tip

When using gdm as display manager remember to delete the file /archiso/airootfs/etc/motd from your system. That files comes originally from Arch Linux.
To avoid waiting for every login and this nice look.
https://imgur.com/a/EvCN4pm


