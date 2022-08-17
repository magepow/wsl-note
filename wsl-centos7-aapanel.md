I. WSL-AAPanel note: 

1. Update system Centos

```
	yum update -y
```
2. Fix error systemctl in WSL
note: run this if update system linux

```
	mv /usr/bin/systemctl /usr/bin/systemctl.old && rm -rf /usr/bin/systemctl
	curl https://raw.githubusercontent.com/gdraheim/docker-systemctl-replacement/master/files/docker/systemctl.py > /usr/bin/systemctl
	chmod +x /usr/bin/systemctl
```

3. Set hostname

```
	hostname srv.magento2.com
```
4. Install

```
	yum install nano -y
	yum install wget -y
	cd /usr/local/src/
	yum install -y wget && wget -O install.sh http://www.aapanel.com/script/install_6.0_en.sh && bash install.sh aapanel
```
5. Start Use

```
service bt stop
Start
service bt start
Restart
service bt restart
```