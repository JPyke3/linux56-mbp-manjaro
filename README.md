# mbp-manjaro-kernel

The Manjaro Kernel built with the latest and greatest kernel patches for T2 Macbooks 2018+ 

mbp-manjaro-iso: ~coming very soon~

All Drivers/Patches Featured:
 * Keyboard, Trackpad, Audio and Suspend: https://github.com/MCMrARM/mbp2018-bridge-drv
 * Arch Linux Kernel Patches (For Driver Above): https://github.com/aunali1/linux-mbp-arch
 * DKMS Module for loading Patches: https://github.com/aunali1/apple-bce-arch
 * Most Recent WiFi Patch: https://github.com/mikeeq/mbp-fedora-kernel
 
 ## Building
 You need to be running either an Arch Linux or Manjaro system to compile the Kernel
 
 Clone the Repository:
 ```
 git clone https://github.com/JPyke3/mbp-manjaro-kernel
 cd mbp-manjaro-kernel
 ```
 Make the Package:
 ```
 makepkg -s
 ```
 Your new Kernel Package will be located in the same directory after compilation (If you are doing this on the mbp itself it can be an hour and a half upwards)
 
 Optionally, if you want to make and install the package to your system:
 ```
 makepkg -si
 ```
 ## TODO
 - [ ] CI
 - [ ] Integrate Patches into Kernel Directly
 - [ ] Improve this README
