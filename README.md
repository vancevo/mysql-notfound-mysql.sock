THIS SOLUTION WORKS FOR ME WHEN I type `mysql -u root -p`

ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/tmp/mysql.sock' (2)

OR

mysql.server-264-kill-No-such-process IN XAMPP


1. Check if the port used by mysql is occupied by a service already (MySql often uses port 3306)
    - sudo lsof -i :3306
=> IT GIVE U <PID> of sql

2. The sudo kill -9 command is used to forcefully terminate a process
    - sudo kill -9 <PID>

3. Restart mysql

`THE OTHER WAY`

1. Check if the port used by mysql is occupied by a service already (MySql often uses port 3306)
    - sudo lsof -i :3306
=> IT GIVE U <PID> of sql

2. GO TO XAMPP, AND CONFIG THE SQL BY PORT <PID> of sql of step 1
