# Zabbix Template for Asus WRT Merlin Routers

<strong>
  If you want to monitor your router using a Zabbix server, this template offers some useful monitoring items.
</strong>


<BR><BR><strong>REQUIREMENTS</strong>

<UL>
  <LI>Asus WRT Router with Merlin firmware</LI>
  <LI>Entware installed</LI>
  <LI>Zabbix agent installed</LI>
      <UL>
        <LI>Agent installation: <a href=https://www.snbforums.com/threads/rt-ac86u-with-zabbix-agent.64343/#post-587787>SNB Forum topic</a></LI>
      </UL>
  <LI>Zabbix agent configuration</LI>
      <UL>
        <LI>Configure file with your router parameters</LI>
        <LI><code>AllowRoot=1</code> parameter<i>(necessary for advanced temperature checks)</i></LI>
        <small><i><a href=https://www.zabbix.com/forum/zabbix-troubleshooting-and-problems/402023-zabbix-agent-system-run>Zabbix forum discussion</a></i></small>
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
  <LI>Template Module Linux network interfaces by Zabbix agent
  <LI>Template Module Zabbix agent
</OL>


<BR><strong>AVALIABLE ITEMS</strong>
<OL>
  <LI>Available memory
  <LI>Connected clients
  <LI>CPU idle time
  <LI>CPU idle time: CPU utilization
  <LI>DHCP Leases
  <LI>Template Module Zabbix agent: Host name of Zabbix agent running
  <LI>HTTP Performance
  <LI>HTTPS Performance
  <LI>Template Module ICMP Ping: ICMP loss
  <LI>Template Module ICMP Ping: ICMP ping
  <LI>Template Module ICMP Ping: ICMP response time
  <LI>Load average (1m avg)
  <LI>Load average (5m avg)
  <LI>Load average (15m avg)
  <LI>Maximum number of processes
  <LI>Memory utilization
  <LI>NTP Performance
  <LI>Number of CPUs
  <LI>Number of processes
  <LI>Number of running processes
  <LI>Operating system
  <LI>SSH service is running
  <LI>System local time
  <LI>System name
  <LI>System uptime
  <LI>Temperature CPU
  <LI>Temperature Wireless 2.4GHz
  <LI>Temperature Wireless 5.0GHz
  <LI>Total memory
  <LI>Template Module Zabbix agent: Version of Zabbix agent running
  <LI>Template Module Zabbix agent: Zabbix agent availability
  <LI>Template Module Zabbix agent: Zabbix agent ping
  <LI><i>Network discovery items</i>
</OL>


<BR><strong>TESTED AS IS</strong>
<BR>
<strong><i>
  This template was tested only with an Asus RT-AC86U router running a Asus Merlin firmware.
  It should work with other Asus routers as well
</i></strong>
