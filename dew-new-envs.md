[https://jira.gtech.com/jira/browse/DEWB-58559]
qe | DEWB-58565

vsphere_hostname: plwawvc01.gtk.gtech.com
datacenter: "WarsawTC_PDC_R&D"
cluster: WarsawTC_BDC_01
folderpath: /WarsawTC_PDC_R&D/vm/SITES/WESTLOTTO/q?
default_datastore_name: BDC_FAS8060_01_VMWARE_DATASTORE_CLUSTER
default_network: VDS1_80_22BIT
default_security_group: aws-only
default_patchlevel: q4-2022

- acgs
- connect
- esout
- esb2b
- estegateway
- pnp
- portal

# qa duplex
I need - 2 static ips for dbs
dewqfwaesdb01
dewqfwaesdb02

dewdewaesdb-vip
dewdewaescb2b-vip
dewdewaesdb-schedule-vip
dewdewaesesdb5-vip
dewdewaesdb01-hadr
dewdewaesdb02-hadr


WarsawTC_BDC_01        - host cluster
BDC_FAS8060_01_VMWARE_DATASTORE_CLUSTER              - datastore cluster
172.30.177.35                 dewqfwaesdb-vip                         maciej.wawrzynczuk@igt.com, 2023.12.04
172.30.177.36                 dewqfwaescb2b-vip                      maciej.wawrzynczuk@igt.com, 2023.12.04
172.30.177.37                 dewqfwaesdb-schedule-vip              maciej.wawrzynczuk@igt.com, 2023.12.04
172.30.177.39                 dewqfwaesesdb5-vip                    maciej.wawrzynczuk@igt.com, 2023.12.04
172.30.177.47                 dewqfwaesdb01-hadr                  maciej.wawrzynczuk@igt.com, 2023.12.04
172.30.177.96                 dewqfwaesdb02-hadr                  maciej.wawrzynczuk@igt.com, 2023.12.04 

[mwawrzynczuk@poluise02 dew]$ cat data/env/wa.yaml
---
puppet_master_name: dewxawacfgmgt01
puppet_master_domain: inf4407.igt.com
puppet_master_ip: 172.30.81.12
satellite_name: infxarirhns
satellite_domain: inf4407.igt.com
satellite_ip: 172.30.180.126
nxprxy_name: nexuspro
nxprxy_domain: inf4407.igt.com
nxprxy_ip: 10.203.1.10
network_management_host: a32xarivtlb01
network_management_ip: 10.17.65.24


[mwawrzynczuk@poluise02 dew]$ cat inventory/group_vars/wa.yaml
---
vsphere_hostname: plwawvc01.gtk.gtech.com
datacenter: "WarsawTC_PDC_R&D"
cluster: WarsawTC_BDC_01
folderpath: /WarsawTC_PDC_R&D/vm/SITES/WESTLOTTO/dx
default_datastore_name: BDC_FAS8060_01_VMWARE_DATASTORE_CLUSTER
default_network: VDS1_80_22BIT
default_security_group: aws-only
default_patchlevel: q4-2022
