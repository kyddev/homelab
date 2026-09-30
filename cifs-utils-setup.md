Source: https://wiki.futo.org/index.php/Introduction_to_a_Self_Managed_Life:_a_13_hour_&_28_minute_presentation_by_FUTO_software



create the files on the VM using:
sudo mkdir /filename

set permissions:
sudo chown -R $USER:$USER /filename
sudo chmod 755 /filename

verify with:
ls -l /

add cifs mount:
sudo nano /etc/fstab

add samba share in fstab:
//192.168.68.101/path/to/file /file cifs uid=1000,gid=1000,username=username,password=password,iocharset=utf8 0 0

restart and mount the service:
sudo systemctl daemon-reload
sudo mount -a

