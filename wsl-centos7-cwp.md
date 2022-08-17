I. WSL-CWP note: 

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
	wget http://centos-webpanel.com/cwp-el7-latest
	sh cwp-el7-latest
```