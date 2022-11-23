# unifi-zabbix-snmpv3
Unifi AP Zabbix SNMPv3  
based on Alex Mouras work https://share.zabbix.com/network_devices/ubiquiti/unifi-snmp-2019-v1-1  

Ubiquity Controller > Settings > Services > SNMP v3 > enable, set $username and $passwort  

Zabbix settings
6.0
SNMP version: SNMPv3
Security name: $username
Security level: authPriv
Authentication protocol: SHA1
Authentication passphrase: $passwort 
Privacy protocol: AES128
Privacy passphrase: $passwort

4.0
Zabbix > Macro >   
{$SNMP_USERNAME} <= username set in controller   
{$SNMP_AUTHPASS} & {$SNMP_PRIVPASS} <= password set in controller   
