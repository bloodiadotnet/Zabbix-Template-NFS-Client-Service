# Zabbix Template NFS Client Service
[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/bloodia/Zabbix-Template-NFS-Client-Service/blob/master/LICENSE)
[![Build Status](https://travis-ci.org/bloodia/Zabbix-Template-NFS-Client-Service.svg?branch=master)](https://travis-ci.org/bloodia/Zabbix-Template-NFS-Client-Service)
[![Maintainability](https://api.codeclimate.com/v1/badges/bdd3c97a75e82f8218ab/maintainability)](https://codeclimate.com/github/bloodia/Zabbix-Template-NFS-Client-Service/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/bdd3c97a75e82f8218ab/test_coverage)](https://codeclimate.com/github/bloodia/Zabbix-Template-NFS-Client-Service/test_coverage)

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
### Script
- Create directory "/usr/local/bin" and copy "Custom Script" file (py) to inside.  
- Change "Custom Script" file (py) to 555 or dr-xr-xr-x using chmod.  

### UserParameter Config
- Copy "UserParameter Config" file (conf) to /etc/zabbix/zabbix_agentd.d and restart Zabbix agent.  

### Template
- Import the template file (xml) and assign it to the host monitored.

## Author
[@bloodia](https://twitter.com/bloodiadotnet)
