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

