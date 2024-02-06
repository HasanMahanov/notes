## eger biz suid icazelerine baxarken suid-env gormusukse
    strings /usr/local/bin/suid-env
## daha sonra gcc ile emri runlayiriq 
    gcc -o service /home/user/tools/suid/service.c
## ve PATH a /usr/local/bin elave edirik
    PATH=.:$PATH /usr/local/bin/suid-env
## ve artiq ROOTSAN


