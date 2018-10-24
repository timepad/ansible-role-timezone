##### Description
Simple ansible role for setting timezone  
Also restarts cron daemon and other dependent daemons if specified  

##### Settings

Setting timezone:
``` 
timezone: UTC
```
Overriding cron daemon service name (by default cron on debian and crond on rhel):
```
timezone_cron_daemon: crond
```
Adding services to restart in case of timezone change:
```
timezone_services_restart:
  - mysql
  - php7.2-fpm
```
