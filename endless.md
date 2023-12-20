# dew gw
10.94.9.198 dewp1s1igtgw01.prod.delot.de dewp1s1igtgw01 dew-pdc
10.94.10.198 dewc1s1igtgw21.test.delot.de dewc1s1igtgw21 dew-cat
10.94.11.198 dewc3s1igtgw21.ftest.delot.de dewc3s1igtgw21 dew-ftest
dewc1s1utl21

# DB
```
DB2_HADR_ESDB_1 65001/tcp
DB2_HADR_ESDB_2 65002/tcp
DB2_HADR_SCHEDULE_1 65007/tcp # HADR for SCHEDULE
DB2_HADR_SCHEDULE_2 65008/tcp # HADR for SCHEDULE
DB2_HADR_ESCB2B_1 65011/tcp # HADR for ESCB2B
DB2_HADR_ESCB2B_2 65012/tcp # HADR for ESCB2B
DB2_HADR_ESDB5_1 65013/tcp # HADR for ESDB5
DB2_HADR_ESDB5_2 65014/tcp # HADR for ESDB5
```

```
yum update --disablerepo='*' --enablerepo=rhel7u9  --enablerepo=security-q2-2023-optional-rhel7u9  --enablerepo=security-q2-2023-rhel7u9  --enablerepo=security-q2-2023-rhn-tools-rhel7u9  --enablerepo=security-q2-2023-supplementary-rhel7u9  --exclude 'pdksh*,ksh*,httpd*,*openldap*,mod_ssl*,freeradius*,*java*,*jdk*,*puppet*,*tomcat*,*fop*'
```

# DES mail
swzq8waacon01 	

idm
rhnp
capsule


# Thu patching
q3-2023
ssh -N -L 8888:thucvircnt3:443 thucat


thucaraut03:thucesmm2:thucggw3:thucnetbck3:thuctivoli3
```
yum update --disablerepo='*' --enablerepo=rhel6u10  --enablerepo=security-q3-2023-els-rhel6u10  --exclude 'pdksh*,ksh*,httpd*,*openldap*,mod_ssl*,freeradius*,*java*,*jdk*,*puppet*,*tomcat*,*fop*'
yum update --disablerepo='*' --enablerepo=rhel7u9  --enablerepo=security-q3-2023-optional-rhel7u9  --enablerepo=security-q3-2023-rhel7u9  --enablerepo=security-q3-2023-rhn-tools-rhel7u9  --enablerepo=security-q3-2023-supplementary-rhel7u9  --exclude 'pdksh*,ksh*,httpd*,*openldap*,mod_ssl*,freeradius*,*java*,*jdk*,*puppet*,*tomcat*,*fop*'
```

# bck interfaces 10 in 3rd octet
1. remove from OS
2. remove from esxi
3. update icha

dewc1s1arte21  | 2
dewc1s2arte22  | 2
dewc1s1esdb21  | 2
dewc1s2esdb22  | 2
dewc1s1gware21 | 2
dewc3s1arte21  | 2
dewc3s1esdb21  | 2

# des ecc
```
sed -i 's/<signAlgo>16/<signAlgo>64/g' /usr/local/gtech/eseries/fsu/fsu.config.xml
/usr/local/gtech/eseries/fsu/fsu.sh statusBackgroundSign
/usr/local/gtech/eseries/fsu/fsu.sh stopBackgroundSign
/usr/local/gtech/eseries/fsu/fsu.sh startBackgroundSign
``` 
dessftp3 
dessftp4
dessftp5
dessftpd3	
dessftpd4
dessftpd5
desnfs3	
desnfs4	
desnfs5	
destivoli3
destivoli4
desggw3	
desggw4
