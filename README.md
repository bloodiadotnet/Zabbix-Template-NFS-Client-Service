# Zabbix Template NFS Client Service
[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/bloodiadotnet/Zabbix-Template-NFS-Client-Service/blob/master/LICENSE)

## Overview
Monitoring client side NFS mount points with Zabbix template.  

## Requires
### OS
- CentOS 5.x - 7.x

### Zabbix
- 3.4
- 4.0

### Python
- 2.6
- 2.7
- 3.3
- 3.4
- 3.5
- 3.6

### Python Modules
- json
- subprocess
- re
- argparse

## Script Usage
```
usage: lld-nfs.py [-h] [-v] [-t FSTYPE] [-n FSNAME]

optional arguments:
  -h, --help            show this help message and exit
  -v, --version         show version and exit
  -t FSTYPE, --fstype FSTYPE
                        select virtual file system type
  -n FSNAME, --fsname FSNAME
                        select virtual file system name

for example: /usr/local/bin/lld-nfs.py -t 'nfs' -n '/data'
```

## How to Install
### Custom Script
- Create directory "/usr/local/bin" and copy "Custom Script" file (py) to inside.  
- Change "Custom Script" file (py) to 555 or dr-xr-xr-x using chmod.  

### UserParameter Config
- Copy "UserParameter Config" file (conf) to /etc/zabbix/zabbix_agentd.d and restart Zabbix agent.  

### Template
- Import the template file (xml) and assign it to the host monitored.

## Author
[@bloodiadotnet](https://twitter.com/bloodiadotnet)
