# smb
smb server for raspberry pi and jetson nano 

sudo apt install samba
whereis samba

sudo vi /etc/samba/smb.conf

#เพิ่มการตั้งค่าไว้ล่างสุด
[NameYourFolder]
    comment = Samba on Ubuntu
    path = /home/pi
    read only = no
    browsable = yes

sudo service smbd restart

sudo smbpasswd -a pi
