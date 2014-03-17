# Resizing Partitions for ArchLinux on VirtualBox

## Setup
1. ArchLinux (2014.03.01 for Intel 32bit was used for this example)
2. Oracle VirtualBox (4.2.12 running on Windows 7 64-bit was used for this 
	example)

## Goal
1. Increase Virtual Box virtual disk size for an existing ArchLinux virtual 
	machine (VM).
2. Grow the existing ArchLinux root partition to use the newly added disk space.


## Steps
*Note* - This process only works with VDI-based disk images. 

1. If running, shutdown the ArchLinux VM.
2.  For safety, clone the VDI file to make a backup of the existing system:
	* Open VirutalBox
	* Select the ArchLinux virtual machine
	* From the main menu, select Machine -> Clone
	* When prompted, select "Full Clone"
	* Wait for the VM cloning process to complete
3. Modify the VDI disk for the original VM :
	* Open Command Prompt (Windows) or Terminal (OS X)
	* Navigate to where your VM is located on the host system
		+ Windows: This is usually c:\Users\username\VirtualBox VMs\vmname
		+ OS X: This is usually /Users/username/Documents/VirtualBox VMs/vmname

## Sources
[vbox8]: https://www.virtualbox.org/manual/ch08.html#vboxmanage-modifyvdi "VirualBox Manual. Chapter 8. VBoxManage. Oracle Corporation. 2013"

## Ideas
1. Write a program that can automate this under any host. It must do the following:
	* Query VM size as an option
	* Back up VDI before resize
	* Resize VDI using VBoxManage
	* Automate growfs/gparted section
	* Could this be made smaller? Use a UEFI image?

Last Modified: 17 Mar 2014 