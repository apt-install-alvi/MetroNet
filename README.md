# MetroNet
A network system prototype for 3 Bangladeshi Metro Rail Stations encompassing the Uttara region : Uttara North, Uttara South and Uttara Center.
Each station has 3 distinct departments:
1. Train Operations - contains PCs that represent Emergency Operation and Regular Operation Systems.
2. Ticketing - contains PCs that represent Machine Ticketing and Manual Ticketing systems and a server that represents Ticket Log Storage
3. Security - contains two servers that represent Security Footage Storage and backups.

The stations are connected to each other via a Ring topology as well as through a Central System via a Star topology. The Central System contains a dedicated PC and Server for central management.
All departments of a specific station can communicate with the corresponding department of another station. No department within a station can directly access its Security System. The Central System has access to all departments.

The system allows the following:
- Shorter hop distances by travelling through the centre as well as backup paths should the central system ever fail due to the Ring+Star topology
- Dynamic IP assignment for all devices through VLSM and DHCP
- Department segregation through VLAN
- Dynamic Routing via OSPF
- Connection restriction with the help of Extended ACL
  
The overall system is designed to be scalable.

## Contributors
[Alvi Binte Zamil](https://github.com/apt-install-alvi) : Topology Setup

[Than Than Thay](https://github.com/Thay-bleh) : VLAN and Inter-VLAN routing

[Lt Sizdatul Karim Evan](https://github.com/SKEvan) : VLSM and DHCP configuration

[Sabit Siraji](https://github.com/Sabit166) : OSPF routing

[Afia Fahmidha Zaman](https://github.com/afiafahmidha) : Extended ACL implementation
