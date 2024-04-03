### Fix Ubuntu Grub Issue 
	** Grub Rescue Issue Fixing

### In my case It was Extending Dual Boot Ubuntu Partision Extending .
	** After Extending the Partision Grub Issue Happens

### Lets Fix the Grub Rescue Issue
	* ls (This will show all the partision)
	* Now ls (hd0, msdos7)/ (Checking if it has boot folder or not)
	* now do it for other for findng Boot loaded folder In my case it was
	* ls (hd0, msdos7)/ 
	* set prefix=(hd0,msdos7)/boot/grub
	* set root=(hd0,msdos7)
	* insmod normal
	* normal
	* Then It will solve Grub Rescue Issue 
	* Now go the the ubuntu System and Open Terminal
	* We need to make this Fix Permanent
	* Type the following command
	* sudo update-grub
	* sudo grub-install /dev/sda
	* sudo reboot
	* We are done Now


### Here is The Command List One after Another

```cmd

ls

ls (hd0, msdos7)/ 

set prefix=(hd0,msdos7)/boot/grub

set root=(hd0,msdos7)

insmod normal

normal

sudo update-grub

sudo grub-install /dev/sda

sudo reboot

```

