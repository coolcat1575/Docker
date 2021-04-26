# My Docker configuration for the following applications

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
