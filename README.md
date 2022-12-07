# MikroTik Configuration Files

MikroTik configuration files for quick router setup. 

## Terminal

```
/tool fetch url="https://raw.githubusercontent.com/pkgstore/mikrotik-conf/main/FILENAME.rsc" dst-path="ros.FILENAME.rsc"
/tool fetch url="https://curl.se/ca/cacert.pem" dst-path="ros.cacert.pem"
/system reset-configuration no-defaults=yes skip-backup=yes run-after-reset="ros.FILENAME.rsc"
/certificate import file-name="ros.cacert.pem" passphrase="" name="ROS"
```
