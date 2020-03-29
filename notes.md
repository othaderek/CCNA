# CCNA Notes

## Network Fundamentals ICND1, Section 1

This is a section about network fundamentals inculding `supermodels`

### OSI and TCP/IP

OSI and TCP/IP are both conecptual models that characterise and standardise the communication functions of a telecommunication or computing system without regard to their underlying internal structure and technology.

OSI consists of 7 layers:

7 - Application
6 - Presentation
5 - Session
4 - Transport
3 - Network
2 - Data Link
1 - Physical

TCP/IP consists of 5 layers:

5 - Application (5-7 of OSI, includes Telnet, FTP, and SMTP)
4 - Transport (TCP and UDP)
3 - Network
2 - Data Link
1 - Physical


### Ethernet cables
They are either UTP or STP
UTP stands for Unshielded Twisted Pair
STP stands for Shielded Twisted Pair

They are twisted because twisting minimizes the effect of EMI, electromagnetic interference

UTP are more common and durable.
STP are less durable and more expensvie and better in theory

Fiber optic gets rid of above problems

#### Copper based standards
IEEE standards
802.3 - Regular ethernet known as 10BASE-T runs at 10Mbps
802.3u - Fast ethernet 100BASE-T runs at 100Mbps
802.3ab - Gigabit ethernet 1000BASE-T runs at 1000Mbps
802.3an - 10Gig ethernet 10GBASE-T runs at 10Gbps

#### Fiber optic standards
802.3z - Gigabit ethernet 1000BASE-LX runs at 1000Mbps

All of the different ethernet standards use the same frame format

#### Crossover and straight through cabling
Host-to-switch -> Straight through cables, called straigh through cause of pin on host end connects straight through to same numbered pin on switch end

Host   Switch 
1 -----> 1 
2 -----> 2
3 <----- 3
6 <----- 6

Pins 1 and 2 transmit on host and and receive on switch end
Pins 3 and 6 transmit on switch end and receive on host end

For switch to switch we need

Switch   Switch 
3 -----> 1 
6 -----> 2
1 <----- 3
2 <----- 6

Gig Ethernet listen and transmit on pins simultaneously

Switch   Switch
1 <-----> 1
2 <-----> 2
3 <-----> 3
4 <-----> 4
5 <-----> 5
6 <-----> 6
7 <-----> 7
8 <-----> 8

Auto MDI-X
If you need a crossover cable and don't have one you can use Auto MDI-X
Switches need to be Auto MDI-X enabled
On Cisco switch port set speed, duplex, and MDIX to auto on that port you want to use Auto MDI-X





