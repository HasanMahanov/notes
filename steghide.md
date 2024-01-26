## ILK OLARAQ
    steghide embed -cf test.jpg -ef test.txt -sf hazir.jpg

## DAHA SONRA 
steghide extract -sf hazir.jpg

## EGER SIFRE VARSA 
    stegcracker hazir.jpg /usr/share/wordlists/rockyou.txt
