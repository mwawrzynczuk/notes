```
ansible -i "/etc/puppetlabs/code/environments/${puppet_env}/inventory/icha.sh"  "$puppet_env"  -m yum -a "name=glibc-langpack-de state=present" -k
```
