# Can you look at this thing for Steve Schutze wiith IDM on arte22?
uid=1567000057(sschutze) gid=26(prosys) groups=26(prosys),1567000023(operations),2011(gsuper),1567000024(ops-admins),301(gtech)


[mwawrzynczuk@dewc1s1igtgw21 ~]$ ipa user-find sschutze
--------------
1 user matched
--------------
  User login: sschutze
  First name: steve
  Last name: schutze
  Home directory: /home/operations/sschutze
  Login shell: /bin/ksh
  Principal name: sschutze@TEST.DELOT.DE
  Principal alias: sschutze@TEST.DELOT.DE
  Email address: steve.schutze@igt.com
  UID: 1567000057
  GID: 26
  Job Title: IGT OPS
  Account disabled: False


access conf from cat arte22:

[root@dewc1s2arte22 security]# egrep -v  '^#|^$' access.conf
+ : schserv : ALL
+ : schxfer : ALL
+ : prosys : cron crond console vc/1 tty1 127.0.0.1 localhost.localdomain

From prod...

[root@dewp1s1arte01 security]# egrep -v '^#|^$' access.conf
+ : (prosys) : ALL
+ : prosys : ALL
+ : schserv : ALL
+ : schxfer : ALL
+ : prosys : cron crond console vc/1 tty1 127.0.0.1 localhost.localdomain dewp1s1arte01 dewp1s1arte02 dewp1s2arte03 dewp1s2arte04

prod arte s2...

+ : schserv : ALL
+ : schxfer : ALL
+ : prosys : cron crond console vc/1 tty1 127.0.0.1 localhost.localdomain dewp1s1arte01 dewp1s1arte02 dewp1s2arte03 dewp1s2arte04


arte.yaml

---
access::allowgroups: ["(prosys)", "prosys", "schserv", "schxfer"]
