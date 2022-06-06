# Jelastic-Zabbix-server
Installs and configures Zabbix 5 on a new Environment.

The Software Stack is LLSMP so Litespeed and MariaDB (see https://docs.jelastic.com/lemp-llsmp)

The installation is based on centos 7.
The frontend is installed manually so not with an automatic package.
This is done by taking the frontend directly from their gitlab and the addon then downloads it using a zip archive in this github repo.

Additionally the zabbix agent is installed for the node.


# Installation
Simply import this link using the Jelastic JPS Import function:
```
https://raw.githubusercontent.com/panslothda/Jelastic-Zabbix-server/master/main.jps
```

Or copy the content of main.jps into the import window.


# Usage
Once the server is installed you will receive a random password and the default Admin username.

There is also an addon that gets installed with following option:

![Interface](images/interface.png?raw=true)

If you press the update button it installs the new version if available and donwloads the new frontend files from this github repo if they have been published and are added on this github.

Previous config files and frontend are backuped to /opt/zabbix for safekeeping.
