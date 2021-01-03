# Module 4
## Networking Fundamentals
### Task 4.1


Connected 4 PC and a hub 

<img src=".\screenshots\Screenshot_1.jpg" width="80%"/>

Made a subnet through assigning IP addresses to each PC, checked if packets were sent and received 

<img src=".\screenshots\2. ICMP_auto captured.jpg" width="80%"/>
<img src=".\screenshots\PDU_info.jpg" width="80%"/>

Then I erased IP addresses (packets don't go through the subnet without IP addresses)

<img src=".\screenshots\3.Erased IP addresses.jpg" width="80%"/>

Created another topology with 2 hubs

<img src=".\screenshots\4_6PC_2Hubs_1Server.jpg" width="80%"/>

Created project with 4 PC and Switch

<img src=".\screenshots\5.Switch_4PC's.jpg" width="80%"/>

#### The main difference is that hub operates at the 1st OSI level while switch at the 2nd level. Packets from switch transmitted to only one port that specified as a recipient.

2 switches and 8 PC scheme

<img src=".\screenshots\6.2Switches.jpg" width="80%"/>

In order to connect the previous scheme with a router I assigned IP address to router ports and default gateway to each PC

<img src=".\screenshots\7.Router_settings.jpg" width="80%"/>

<img src=".\screenshots\8.default gateway.jpg" width="80%"/>

Packets successfully transmit from one subnet to other

<img src=".\screenshots\9.ROUTER.jpg" width="80%"/>

#### Router operates at the 3rd OSI level using IP addresses whereas switch at 2nd. We are able to connect local networks with each other through router, also, router is adding us other advantages such as NAT, Firewall etc.

pkt files:

<a href="https://github.com/artemfilimonenko/DevOps_online_Kharkiv_2020Q42021Q1/blob/main/m4/task%204.1/pkt%20files/proj1_4PC_1Hub.pkt/">Hub and 4 PC</a>
<a href="https://github.com/artemfilimonenko/DevOps_online_Kharkiv_2020Q42021Q1/blob/main/m4/task%204.1/pkt%20files/4.1_router.pkt/">Router and 2 subnets</a>

