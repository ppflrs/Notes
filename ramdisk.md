To create a ramdisk of 4G:

diskutil erasevolume HFS+ 'ramdisk' `hdiutil attach -nomount ram://8388608`

You can access to the disk via the /Volumes/ folder.

To delete the ramdisk

umount -f /Volumes/$RAMDISK

hdiutil detach /Volumes/$RAMDISK
