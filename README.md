## Zabbix Agent Configuration ##
EnableRemoteCommands=1<br/>
UnsafeUserParameters=1<br/>
Alias=service.discovery.veeam:service.discovery<br/>
UserParameter=vbr[*],powershell -NoProfile -ExecutionPolicy Bypass -File “C:\Program Files\Zabbix Agent\scripts\zabbix_vbr_job.ps1” “$1” “$2” “$3”<br/>