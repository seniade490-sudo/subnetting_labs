# subnetting_labs
These subnetting labs teaches how to subnet in different subnet masks; the diagrams and screenshots are evidence of labs
The I.P address in, 10.1.1.1 and the subnet mask of 255.255.255.0 /24, gives a CIDR of 24; 
The I.P address in, 10.1.2.2 and the subnet mask of 255.255.255.0 /24, gives a CIDR of 24;

They are both on different subnets, send a packet from R1 to R2 would be undeliverable,

changing R1 and R2's, IP address to reside in the same subnet, the ARP and ICMP packet would be initiated.
10.1.1.1 255.255.0.0 /16; 10.1.2.2 255.255.0.0 /16; CIDR = 16 and each packet sent would be able to be delivered.

sh ip int g0/0/0 shows the IP CIDR mask address,
sh run shows the configuration made on each port interface,
sh ip route shows the routing configuration on the router,
debug IP packet = ??

we can create IP's and subnets from 10.1.1.1 255.0.0.0 /8 on R1;
IP and subnets for R2 10.1.2.2 255.0.0.0 /8 on R2;

Packets from r1 would ping across r2 using ICMP and ARP; 
Take a look at the screenshot for the ICMP and ARP packets


