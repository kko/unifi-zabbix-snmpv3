# unifi-zabbix-snmpv3
unifi zabbix snmpv3  
based on Alex Mouras work https://share.zabbix.com/network_devices/ubiquiti/unifi-snmp-2019-v1-1  

Ubiquity Controller > Settings > Services > SNMP v3 > enable, set username and passwort  
Zabbix > Macro >   
{$SNMP_USERNAME} <= username set in controller   
{$SNMP_AUTHPASS} & {$SNMP_PRIVPASS} <= password set in controller   
