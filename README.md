# Pierre's Home server
This guide is aimed at everyone seting up their own home automation server for the first time.
 
Prerequsits: 
- 64 bit capable computer 
- Debian amd64 iso (Get the netinstallation ISO from here https://cdimage.debian.org/debian-cd/current/amd64/iso-cd/ )
- USB memory 4 GB
- Balena Etcher (Get it here https://www.balena.io/etcher/ )
- Basic linux knowledge

Task sequense to install Debian:
- Burn ISO to USB memory with Balena Etcher
- Boot on USB memory and install Debian with notes below
  - Select correct keyboard
  - configure root password
  - Configure new user
  - Remove graphical interface
  - Add SSH Server
- Remove the USB memory and reboot computer

Task sequense to install Docker:
- Log into computer with root user
- run the following command to install wget and unzip: 
```apt install wget unzip ```
- run the following command to download the repository: 
```wget https://github.com/coolcat1575/Docker/archive/refs/heads/main.zip```
- extract the file with: unzip main.zip
run the following command to move the Docker-main folder: mv Docker-main/ /usr/local/Docker
 
 

|Application|Description|Settings|
|-----------|-----------|--------|
|adguardhome|Pi-Hole alternative|Own LAN Address (192.168.200.2)|
|codeserver|Visual Basic Codeserver|Exposes port 8444|                        
|glances|Process explorer|Exposes port 61208|           
|hadb|Home Assistand DB|Exposes port 3306|
|heimdall|Startpage|Exposes port 7080|
|homeassistant|Home Assistant|Network=Host|
|librespeed|Own Speedtest server|Exposes port 8888|
|mqtt|MQTT server used by Hom-Assistant|Network=Host|
|portainer|Manage docker containers|Exposes port 9000|
|postgresserver|Zabbix DB|Exposes port 5432|
|speedtest|Schedules speedtests|Exposes port 8765|
|zabbixagent2|Zabbix Agent 2|Network=Host|
|zabbixserver|Zabbix network monitor server|Network=Host|
|zabbixsnmptraps|Zabbix trap server|Exposes port 162|
|zabbixwebnginx|Zabbix Web Server|Network=Host|
