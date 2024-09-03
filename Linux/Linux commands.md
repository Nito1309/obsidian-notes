#### Show info about disk space usage on file systems
```
sudo df -hTa
```

#### Show filesystems and their associated parameters
It is used by the Linux kernel to mount declared file systems during booting
```
cat /etc/fstab
```

#### Show kernel version
```
uname -r
```

#### List available kernels
```
ls /boot/vmlinuz-*
```

#### Check the GRUB menu entries
```
grep menuentry /boot/grub/grub.cfg
```

#### Open the GRUB configuration file
```
sudo vi /etc/default/grub
```

#### GRUB default bootloader in GNU
Update grub after have made changes in 
```
sudo update-grub
```

#### Set an environment variable executable
```
export PATH="/path/to/executable:$PATH"
```

#### Path to directory you can add new repositories without edit the central file "sources.list"
```
 cd /etc/apt/sources.list.d/
```

#### Print the booted initrd image 
```
ls -l /boot/initrd.img-$(uname -r)
```

#### Stop pop-up to restart the services
They will automatically restart with 'a' value or with 'l' the services that require restart will be listed
```
sed -i "/#\$nrconf{restart} = 'i';/s/.*/\$nrconf{restart} = 'a';/" /etc/needrestart/needrestart.conf
```
