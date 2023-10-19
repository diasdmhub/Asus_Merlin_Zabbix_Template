# Zabbix Template for Asus WRT Merlin Routers

<div align="right">
<a href="./LICENSE">
	<img src="https://img.shields.io/badge/License-GPL3-blue?logo=opensourceinitiative&logoColor=fff" alt="License GPL3">
</a>
<a href="https://github.com/diasdmhub/Asus_Merlin_Zabbix_Template/releases/tag/latest">
	<img src="https://img.shields.io/badge/Version-647-blue?logo=azurepipelines&amp;color=0aa8d2" alt="Latest Version">
</a>
</div>
<BR>


### OVERVIEW
If you want to monitor your Asus SOHO router using a Zabbix agent, this template offers some useful monitoring items, triggers, graphs and more.
It targets Asus WRT routers with the Merlin firmware installed.

The main focus is to monitor specific Asus Merlin Router items. \
For generic Linux items, it is recommended to link your host to the OOTB Linux template which offers multiple items for monitoring, including CPU, memory, disk and bandwidth information.

<BR>


### REQUIREMENTS

- Asus WRT Router with [Merlin firmware](https://www.asuswrt-merlin.net)
- Entware installed
- Zabbix agent installed
  - You can try my [Zabbix Agent installation script](https://github.com/diasdmhub/Zabbix_agent_Asus_Merlin)

<BR>


### SETUP

- Configure the Zabbix Agent configuration file:
  - Use `Server=` parameter with your Zabbix Server IP/Hostname
  - Add `AllowKey=system.run[*]` parameter *(necessary for custom checks)*
  - Add `AllowRoot=1` parameter *(necessary since no Zabbix user is created)* \
  [*Zabbix forum discussion*](https://www.zabbix.com/forum/zabbix-troubleshooting-and-problems/402023-zabbix-agent-system-run)

<BR>

---
### ➡️ [Download (latest)](https://github.com/diasdmhub/Asus_Merlin_Zabbix_Template/releases)
---
#### ➡️ [*How to import templates*](https://www.zabbix.com/documentation/current/en/manual/xml_export_import/templates#importing)
---

<BR>


### TESTED VERSION
- This template was tested only with Asus RT-AC86U / RT-AC87U / RT-AX86U router running an Asus Merlin firmware.
- It should work with other Asus routers as well.
- [*SNBForums original post*](https://www.snbforums.com/threads/asus-merlin-router-with-zabbix-agent.64343)
- [*WEB UI Memory discussion*](https://www.snbforums.com/threads/gui-memory-x-meminfo.68683/#post-645321)

<BR>


### ITEMS

| Name                            |
| ------------------------------- |
| AdGuard Home Status             |
| Conmon CSV                      |
| Conmon CSV: Conmon Jitter       |
| Conmon CSV: Conmon Line Quality |
| Conmon CSV: Conmon Ping         |
| DNS Service IPv4                |
| DNS Service IPv6                |
| Device Model                    |
| Internet IPv4                   |
| Internet IPv6                   |
| Memory WebUI Free               |
| Memory WebUI Total              |
| Memory WebUI Used               |
| NTP Performance                 |
| NTPMerlin CSV                   |
| NTPMerlin CSV: NTPMerlin Drift  |
| NTPMerlin CSV: NTPMerlin Offset |
| Temperature CPU                 |
| Temperature Wireless 2.4GHz     |
| Temperature Wireless 5.0GHz     |
| Web Performance                 |

<BR>


### TRIGGERS

| Name                             |
| -------------------------------- |
| AdGuardHome Status Down          |
| CPU High temperature             |
| CPU High temperature ALERT       |
| Conmon abnormal Ping rise        |
| Conmon reports low line quality  |
| DNS Service IPv4 down            |
| DNS Service IPv6 down            |
| NTP service is down              |
| Web service is down              |
| Wireless 2.4GHz high temperature |
| Wireless 5.0Hz high temperature  |

<BR>


### GRAPHS

| Name                 |
| -------------------- |
| Conmon Response Time |
| Memory WEBUI         |
| NTPMerlin            |
| Temperature          |
| WEB x NTP Perfomance |

<BR>

	
### WEB MONITORING

| Name            |
| --------------- |
| WEB UI Scenario |

<BR>
	
	
### DASHBOARD EXAMPLE
![Graph examples](images/graph_example.png)
