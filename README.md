# unifi-zabbix-snmpv3
Unifi AP Zabbix SNMPv3  
based on Alex Mouras work https://share.zabbix.com/network_devices/ubiquiti/unifi-snmp-2019-v1-1  

Ubiquity Controller > Settings > Services > SNMP v3 > enable, set $username and $passwort  

Zabbix settings<br>
6.0<br>
SNMP version: SNMPv3<br>
Security name: $username<br>
Security level: authPriv<br>
Authentication protocol: SHA1<br>
Authentication passphrase: $passwort<br> 
Privacy protocol: AES128<br>
Privacy passphrase: $passwort<br>

4.0
Zabbix > Macro >   
{$SNMP_USERNAME} <= username set in controller   
{$SNMP_AUTHPASS} & {$SNMP_PRIVPASS} <= password set in controller   
