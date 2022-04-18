# Unattended-Ubuntu
Download the ubuntu iso https://ubuntu.com/download/desktop and unzip the iso using  
```
sudo mount -o loop <Ubuntu-iso> <mnt-dir>
```
Change the folders that are in this repo and then mount again using   
```
mkisofs -D -r -V "UNATTENDED_UBUNTU" -cache-inodes -J -l -b isolinux/isolinux.bin -c isolinux/boot.cat -no-emul-boot -boot-load-size 4 -boot-info-table -o <iso-destination> <mnt-dir>
```
