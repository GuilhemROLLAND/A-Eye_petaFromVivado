# Petalinu From a Vivado Hardware Description File
Guilhem ROLLAND  
Thomas DU BOISROUVRAY  
Elsys Design Rennes  
## Project
Build an IA coded in C on a zybo Z7-20.
## Usefull commands
```bash
petalinux-create -t project --template zynq -n petaFromVivado --> Create the workspace   
petalinux-config --get-hw-description --> Load HDF file   
petalinux-config --> Enter global configuration    
petalinux-config -c rootfs --> Enter rootfs configuration   
petalinux-build --> produce image.ub and rootfs files   
petalinux-package --boot --force --fsbl images/linux/zynq_fsbl.elf --fpga images/linux/*_wrapper.bit --u-boot --> produce BOOT.BIN    
```