# Set ip setiap router
Router 1 (CR) <br>
Ethernet 1: 152.167.10.1/24 <br>
Ethernet 2: 192.168.20.1/24 
 
Router 2 (KJ) <br>
Ethernet 1: 152.167.10.2/24 <br>
Ethernet 2: 192.168.30.1/24 

Router 3 (KHI) <br>
Ethernet 1: 152.167.10.3/24 <br>
Ethernet 2: 192.168.10.1/24 

# Set Ipip Tunnel
Router 1 (CR) <br>
Local address: 152.167.10.1 <br>
destination address: 152.167.10.2 <br>
Tambahkan ip tunnel: 192.168.100.1 

Router 2 (KJ) <br>
Local address: 152.167.10.2 <br>
destination address: 152.167.10.2 <br>
Tambahkan ip tunnel: 192.168.100.1 

Router 3 (KHI) <br>
Local address: 152.167.10.3 <br>
destination address: 152.167.10.2 <br>
Tambahkan ip tunnel: 192.168.100.1 