

Reinstall the GRUB boot loader to your Ubuntu installation in EFI mode this way ...
Boot from the Ubuntu installation media and select Try Ubuntu without installing.
Once on the Live desktop - open a terminal and execute the following commands :

	sudo mount /dev/sd*** /mnt
	sudo mount /dev/sd** /mnt/boot/efi
	for i in /dev /dev/pts /proc /sys /run; do sudo mount -B $i /mnt$i; done
	sudo chroot /mnt
	grub-install /dev/sd*
	update-grub  

Note : sd* = disk | sd** = efi partition | sd*** = system partition
To identify the partitions use GParted (included in the install media).
After completion GRUB will be installed in the separate EFI partition.

http://askubuntu.com/questions/831216/reinstalling-grub2-efi-partition
