## eger hansisa sistemin id-rsa varsa biz artiq hemin sisteme oz atack masinimizda ip adresi ile daxil ola bileriq root kimi 
## (USERDE)
## evvelce biz cat verib hemid id rsa oxuyuruq
## sorna  biz oz atack masinimiza kecirik ve NANO ILE HEMID FAYL ADINDA BIR FAYL YARADIRIQ VE HEMID YAZINI BURA DAXIL edirik
## (KALIDE)'
    ssh -i (ID_RSA-ADINI) -oPubkeyAcceptedKeyTypes=+ssh-rsa -oHostKeyAlgorithms=+ssh-rsa root@10.10.146.185

## VE ARTIQ ROOT KIMI DAXIL OLMUSUQ    
    
