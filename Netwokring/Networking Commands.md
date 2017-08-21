### Networking 

#### Tools:

- [Nmap]()
- [Routing Tables](https://github.com/nairuzabulhul/General-Commands/blob/master/Netwokring/Networking%20Commands.md#routing-tables)
- [MAC Addresses]()
- Switches
- Hubs
-   ARP
- [WireShark]()

__OSI Model__
        
        - Application 
        - Presentation 
        - Session
        - Transport 
        - Network
        - Data Link
        - Physical 
    
    
### Routing Table: 

    __Windows__ : 
        
        route print 

    __Linux__ :
    
        ip route 
        
        route -r  --> display all the routing tables  
        
        rout add  -host IP_address  -gw Degfault_Gateway Interface_Name    
        
        rout del -host IP_address  -gw Degfault_Gateway Interface_Name  
        
    __OSX__:
    
        netstat -r 
        


### MAC Addresses: 

>> Physical Address of the Network Interface Card (NIC)

 __Windows__:
    
        ipconfig /all
        

__Linux__:

        ip addr
        
__OSX__:

      ifconfig 
        
        
### ARP: 

>> Binding IP address with MAC address

   - __ARP Request__ 
   - __ARP Reply__ 

__Windows__

        arp -a
        
__Linux__

    ip neighbor 
    
    arp 
    
__OSX__

    arp 
    


### Hubs:

>> are repeaters forward packets by repeating electrical signals. Hubs send packets to all clients on the network 


### Switches : 

>>  

- __Forwarding Tables__ used to forward packet to the specific client via MAC address
- 


### TCP/UDP

- __TCP__ Transport Control Protocol 
    
    - Slow 
    - Performs handshakes 
    - Checks the arrival of packert

    __Ex: Sending emails, sharing files__

- __UDP__ User Datagram Protocl 

    - Fast 
    - No checking mechanism 

    __Ex: Streaming videos: Nertflix , Skype calls__


#### Nmap







