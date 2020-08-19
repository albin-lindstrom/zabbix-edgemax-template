![](https://i.imgur.com/N6GqEC1.png)

# Zabbix: EdgeMAX Template (SNMPv2)

This template allows you to quickly get up and running with monitoring of Ubiquiti's EdgeRouter line of devices. It allows for auto-discovering of network interfaces and automatically applies appropriate triggers for the discovered network interfaces.

## ⚙️ Installation

1. Select a branch according to your Zabbix version and download the xml.
2. Import *zbx_edgemax_template.xml* to Zabbix (Configuration -> Templates -> Import)
3. Add the template *Template EdgeMAX SNMPv2* to your host and configure 
   1. Add *{$SNMP_COMMUNITY}* to your host's macros and configure it. (default is usually public)
4. Enable the *SNMP* agent on your EdgeMAX device.
   1. Set *SNMP community* to the same value as your macro or the other way around.

## 🏷️ Features
- ✔️ Auto discovering of network interfaces
- ✔️ Monitoring traffic in/out per network interface
- ✔️ Monitoring up/down status per network interface
- ✔️ Monitoring of discarded and error packets per network interface
- ✔️ Monitoring of memory utiliziation of system
- 🔶 Linked with **Template Module Generic SNMPv2**

## Supported models
Updated as of 2020-04-30.
- **EdgeRouter**
  - ER-X
  - ER-5 ( + poe)
  - ER-6 ( + poe)

## Issues
- [Wrong ethernet link status/speed via SNMP](https://community.ui.com/questions/Wrong-ethernet-link-status-speed-via-SNMP/6e50940c-3cc1-4242-9881-5c03e7892ebf)


## License
[MIT](https://choosealicense.com/licenses/mit/)