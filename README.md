# School-Project-wCisco-Equipments
Cisco Packet Tracer diagram introduced on Cisco physical equipments:


![Diagram](https://user-images.githubusercontent.com/98745874/163879472-c4213970-247d-4052-b31c-7af41845f88c.PNG)

💡 Diagram of the project made in Cisco Packet Tracer just for illustration and organization, configurations made on the physical Cisco equipment.

Networks: 'ENTA', 'ALFA' and 'BETA' connected to each other through an encrypted tunnel. (Tun 100 & Tun 200)

'ENTA' equipment will be able to make VOIP communications with 'ALFA & BETA' equipment

'ENTA' can access the 'ALFA & BETA' WEB Server

'ALFA' and 'BETA' equipments will be able to ping 'ENTA' equipment through the encrypted IPSec Tunnel (100 or 200)

StandBy Protocol used between 'ALFA' and 'BETA'

ENTA:

  1. DHCP and VOIP
  2. LACP Protocol between 2 Switches with 2 cables
  3. EIGRP Protocol
  4. VTP (Vlan Trunking Protocol)
  5. STP (Spanning Tree Protocol)
  6. Tun 100 & Tun 200
  
  All traffic goes through Tunnel 100, in case the ALFA router is down, it goes through Tunnel 200.
  
ALFA:

  1. EIGRP
  2. HSRP (StandBy Protocol)
  3. Tun 100
  4. ACL

BETA:
  
  1. EIGRP
  2. HSRP (StandBy Protocol)
  3. Tun 200
  4. ACL

Cisco ASA:

  1. Bridge Interfaces (inside and outside)
  2. DHCP for 'inside' and 'DMZ' interfaces
  3. NAT
  4. ACL's

Cisco Equipment:

  1. Routers 2811 & 2911
  2. Switches 2960-24TT
  3. Cisco ASA 5506
  4. IP Phones 7960
