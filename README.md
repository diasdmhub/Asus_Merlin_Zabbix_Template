# Zabbix Template for Asus WRT Merlin Routers

<strong>
  If you want to monitor your Asus SOHO router using a Zabbix agent, this template offers some useful monitoring items.
</strong>


<BR><BR><strong>REQUIREMENTS</strong>

<UL>
  <LI>Asus WRT Router with Merlin firmware</LI>
  <LI>Entware installed</LI>
  <LI>Zabbix agent installed</LI>
      <UL>
        <LI>Agent installation: <a href=https://github.com/diasdmhub/Zabbix_agent_Asus_Merlin>Zabbix Agent installation script</a></LI>
      </UL>
  <LI>Zabbix agent configuration</LI>
      <UL>
        <LI>Configure file with your router parameters</LI>
        <LI>Add <code>AllowKey=system.run[*]</code> parameter<i> (necessary for custom checks)</i></LI>
        <LI>Add <code>AllowRoot=1</code> parameter<i> (necessary since no Zabbix user is created)</i></LI>
        <small><i><a href=https://www.zabbix.com/forum/zabbix-troubleshooting-and-problems/402023-zabbix-agent-system-run>Zabbix forum discussion</a></i></small>
        <LI>You can try my <a href=https://github.com/diasdmhub/Zabbix_agent_Asus_Merlin>Zabbix Agent installation script</a></LI>
      </UL>
</UL>


<BR><strong>ENABLED</strong>
<UL>
  <LI>Items</LI>
  <LI>Triggers</LI>
  <LI>Graphs</LI>
  <LI>Discovery rules</LI>
</UL>


<BR><strong>LINKED TEMPLATES</strong>
<OL>
  <LI>Template Module ICMP Ping
  <LI>Template Module Linux block devices by Zabbix agent
  <LI>Template Module Linux filesystems by Zabbix agent
  <LI>Template Module Linux network interfaces by Zabbix agent
  <LI>Template Module Zabbix agent
</OL>


<BR><strong>AVALIABLE ITEMS</strong>
<OL>
  <LI>Connected clients
  <LI>CPU idle time
  <LI>CPU idle time: CPU utilization
  <LI>DHCP Leases
  <LI>HTTP Performance
  <LI>HTTP Performance Average
  <LI>HTTPS Performance
  <LI>HTTPS Performance Average
  <LI>Template Module ICMP Ping: ICMP loss
  <LI>Template Module ICMP Ping: ICMP ping
  <LI>Template Module ICMP Ping: ICMP response time
  <LI>Load average (1m avg)
  <LI>Load average (5m avg)
  <LI>Load average (15m avg)
  <LI>Maximum number of processes
  <LI>Template Module Linux memory by Zabbix agent: Total memory
  <LI>Template Module Linux memory by Zabbix agent: Memory utilization
  <LI>Template Module Linux memory by Zabbix agent: Available memory
  <LI>Template Module Linux memory by Zabbix agent: Total swap space
  <LI>Template Module Linux memory by Zabbix agent: Free swap space in %
  <LI>Template Module Linux memory by Zabbix agent: Free swap space
  <LI>Memory WebUI Free
  <LI>Memory WebUI Total
  <LI>Memory WebUI Used
  <LI>NTP Performance
  <LI>NTP Performance Average
  <LI>Number of CPUs
  <LI>Number of processes
  <LI>Number of running processes
  <LI>Operating system
  <LI>Template App SSH Service: SSH service is running
  <LI>System local time
  <LI>System name
  <LI>System uptime
  <LI>System description
  <LI>Temperature CPU
  <LI>Temperature Wireless 2.4GHz
  <LI>Temperature Wireless 5.0GHz
  <LI>Template Module Zabbix agent: Version of Zabbix agent running
  <LI>Template Module Zabbix agent: Zabbix agent availability
  <LI>Template Module Zabbix agent: Zabbix agent ping
  <LI>Template Module Zabbix agent: Host name of Zabbix agent running
  <LI>Internet IPv4
  <LI>Internet IPv6
  <i>
    <LI>Network discovery items
    <LI>Mounted filesystem discovery
    <LI>Block devices discovery
  </i>
</OL>


<BR><strong>GRAPH EXAMPLE</strong>
  <BR><BR><img src="zabbix_graph_example.png" alt="Graph examples">

<BR>
<UL>
  <LI><a href=https://www.snbforums.com/threads/gui-memory-x-meminfo.68683/#post-645321>WEB UI Memory discussion</a></LI>
</UL>


<BR><strong>TESTED AS IS</strong>
<BR>
<strong><i>
  This template was tested only with Asus RT-AC86U / RT-AC87U / RT-AX86U router running a Asus Merlin firmware.
  It should work with other Asus routers as well
</i></strong>
