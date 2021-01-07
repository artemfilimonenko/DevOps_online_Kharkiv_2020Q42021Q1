# Module 4
## Networking Fundamentals
### Task 4.2

#### The labwork consists of 3 tasks.

#### Task 4.2.1

*It was necessary to build a corporate network that contains of 2 buildings with 2 floors in each. 
Horizontal floor subnetwork consists of one working group of 5 computers.*

I built the network choosing  1 router and 4 switches, each of which linked with 5 PC.

Adding 2 fiber interfaces to the router

<img src=".\screenshots 4.2.1\1.Adding ports to the router.jpg" width="80%"/>

Adding fast ethernet interfaces to each switch

<img src=".\screenshots 4.2.1\2. Adding ports to each switch.jpg" width="80%"/>

Configuring static IP addresses and appropriate gateway for each PC

<img src=".\screenshots 4.2.1\3.IP_addresses to all devices.jpg" width="80%"/>

Checking if packets transmit through the network
<img src=".\screenshots 4.2.1\4.tracert from different subnets.jpg" width="80%"/>
<img src=".\screenshots 4.2.1\5.Network works.jpg" width="80%"/>


#### Task 4.2.2

*The task was to build a network that contains of one 4 floors building. Floor's horizontal subnetwork consists of two workgroups with 3 and 5 PC. Accomplish network logical structuring on 8 subnetworks.*

Building the network through 5 switches and 30 workstations
<img src=".\screenshots 4.2.2\1. Built a network.jpg" width="80%"/>

Implementing  VLANs, access mode on internal switches and trunk mode on the external 
<img src=".\screenshots 4.2.2\2.VLAN creating.jpg" width="80%"/>
<img src=".\screenshots 4.2.2\3.adding FA ports to VLAN.jpg" width="80%"/>
<img src=".\screenshots 4.2.2\4.Adding trunk.jpg" width="80%"/>

Sending ICMP packets within one subnet 
<img src=".\screenshots 4.2.2\ICMP between 1 subnet.jpg" width="80%"/>

Ping between different subnetworks 
<img src=".\screenshots 4.2.2\ICMP between 1 subnet and dif subnets.jpg" width="80%"/>

##### As we may see ICMP packets transmit within the same subnetwork, but we can't reach a workstation from different subnetwork

#### Task 4.2.3
 
*Create a local network based on 5 one-story buildings. One buildng = one workgroup of 6 PC. The network should be based on an one port router.*

Defining the network structure of 5 subnetworks. Implementing VLANs 10, 20, 30, 40, 50.

<img src=".\screenshots 4.2.3\1.Built a network.jpg" width="80%"/>

Assigning IP addresses and appropriate gateway for the each PC
<img src=".\screenshots 4.2.3\2.IP, Gateway assigning.jpg" width="80%"/>

Trying to send an ICMP packet between VLANs 

<img src=".\screenshots 4.2.3\3.Ping between vlans.jpg" width="80%"/>

Changing internal switches ports into access
<img src=".\screenshots 4.2.3\4.setting ports on switches (ACCESS).jpg" width="80%"/>

Changing ports of the external switch into trunk
<img src=".\screenshots 4.2.3\5.Setting central switch.jpg" width="80%"/>
<img src=".\screenshots 4.2.3\6.Show interfaces trunk.jpg" width="80%"/>

Configuring subnetworks on the router 
<img src=".\screenshots 4.2.3\7.Configuring router.jpg" width="80%"/>

Sending ICMP to the router subinterface and between different VLANs

<img src=".\screenshots 4.2.3\8.ICMP to router.jpg" width="80%"/>
<img src=".\screenshots 4.2.3\9.Ping between different vlans.jpg" width="80%"/>

As we may see packets are transmitting to the certain subinterface, also we can ping workstations between VLANs. 

pkt files:
https://github.com/artemfilimonenko/DevOps_online_Kharkiv_2020Q42021Q1/tree/main/m4/task%204.2/pkt%20files




