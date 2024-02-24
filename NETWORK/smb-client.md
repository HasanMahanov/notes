# ilk olaraq smb shelli ile daxil oluruq ve icerisindeki fayl ve qovluqlara baxiriq
    └─$ smbclient -L //10.10.188.204/
# daha sonra istediyimiz fayli secirik ve 

    └─$ smbclient  //10.10.188.204/qovluq(fayl)
# user ile ise 
    └─$ smbclient  //10.10.188.204/qovluq -U 'Anonymous'
