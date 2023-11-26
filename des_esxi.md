```
/vmfs/volumes/datastore_pdc_cat_1/des-esxi/ESXi670-202111001.zip
/vmfs/volumes/datastore_pdc_cat_1/des-esxi/ESXi670-202201001.zip
/vmfs/volumes/datastore_pdc_cat_1/des-esxi/ESXi670-202206001.zip
/vmfs/volumes/datastore_pdc_cat_1/des-esxi/ESXi670-202207001.zip
/vmfs/volumes/datastore_pdc_cat_1/des-esxi/ESXi670-202210001.zip

esxcli software sources profile list -d /vmfs/volumes/datastore_pdc_cat_1/des-esxi/ESXi670-202111001.zip
esxcli software sources profile list -d /vmfs/volumes/datastore_pdc_cat_1/des-esxi/ESXi670-202201001.zip
esxcli software sources profile list -d /vmfs/volumes/datastore_pdc_cat_1/des-esxi/ESXi670-202206001.zip
esxcli software sources profile list -d /vmfs/volumes/datastore_pdc_cat_1/des-esxi/ESXi670-202207001.zip
esxcli software sources profile list -d /vmfs/volumes/datastore_pdc_cat_1/des-esxi/ESXi670-202210001.zip

ESXi-6.7.0-20211104001-standard
ESXi-6.7.0-20220104001-standard
ESXi-6.7.0-20220604001-standard
ESXi-6.7.0-20220704001-standard
ESXi-6.7.0-20221004001-standard

esxcli software profile update -d /vmfs/volumes/datastore_pdc_1/des-esxi/ESXi670-202111001.zip -p ESXi-6.7.0-20211104001-standard --dry-run
esxcli software profile update -d /vmfs/volumes/datastore_pdc_1/des-esxi/ESXi670-202201001.zip -p ESXi-6.7.0-20220104001-standard --dry-run
esxcli software profile update -d /vmfs/volumes/datastore_pdc_1/des-esxi/ESXi670-202206001.zip -p ESXi-6.7.0-20220604001-standard --dry-run
esxcli software profile update -d /vmfs/volumes/datastore_pdc_1/des-esxi/ESXi670-202207001.zip -p ESXi-6.7.0-20220704001-standard --dry-run
esxcli software profile update -d /vmfs/volumes/datastore_pdc_1/des-esxi/ESXi670-202210001.zip -p ESXi-6.7.0-20221004001-standard --dry-run
```


syslog
sig
este
esc
db


skip:
esaweb
