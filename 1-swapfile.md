###__STEPS TO CREATE / EDIT /REMOVE SWAPFILE__

1. __check swap__ =
   >`sudo swapon --show`

2. __turn swap off__ =
   > `sudo swapoff -v /swapfile`

3. __create file__ =
   >` sudo fallocate -l 4G /swapfile`

4. __give permission__ =
   >`sudo chmod 600 /swapfile` 

5. __create swap file system__ = 
   >`sudo mkswap /swapfile`

6. __turn on swap__ =
   >` sudo swapon /swapfile`

7. __remove swapfile__=
   >`  sudo rm /swapfile`

8. __swapfile mention location__ =
   > /etc/fstab (edit this file with root access with editor of your choice and edit or remove entry [not file])

9. __check swappiness value__ =
    >` cat /proc/sys/vm/swapiness`

10. __change swappiness__ = 
    >`sudo nano /etc/sysctl.conf  {add line "vm.swappiness=10" replace 10 by your number }`
##Note:
> less swappiness== more ram use 


>__its better to delete and create new swap file instead of editing__
