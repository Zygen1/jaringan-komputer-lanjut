# Set ip setiap router
Router 1 (CR) <br>
Ethernet 2: 192.168.30.1/24 <br>
Ethernet 3: 10.10.10.1 <br>
Ethernet 4: 20.20.20.1
 
Router 2 (KJ) <br>
Ethernet 2: 192.168.10.1/24 <br>
Ethernet 3: 20.20.20.2 <br>
Ethernet 4: 30.30.30.2

Router 3 (KHI) <br>
Ethernet 2: 192.168.20.1/24 <br>
Ethernet 3: 10.10.10.2 <br>
Ethernet 4: 30.30.30.1

# Lakukan DHCP Server setiap router
Router 1 (CR) <br>
DHCP Server -> Ethernet 2

Router 2 (KJ) <br>
DHCP Server -> Ethernet 2

Router 3 (KHI) <br>
DHCP Server -> Ethernet 2

# Set Interface Routing RIP
Router 1 (CR) <br>
Tambahkan Interface all | Receive v1-2 | Send v2 <br>

Router 2 (KJ) <br>
Tambahkan Interface all | Receive v1-2 | Send v2 <br>

Router 3 (KHI) <br>
Tambahkan Interface all | Receive v1-2 | Send v2 <br>

# Set Network Routing RIP
Router 1 (CR) <br>
Tambahkan network: <br>
192.168.30.0 <br>
10.10.10.0 <br>
20.20.20.0

Router 2 (KJ) <br>
Tambahkan network: <br>
192.168.10.0 <br>
20.20.20.0 <br>
30.30.30.0

Router 3 (KHI) <br>
Tambahkan network: <br>
192.168.20.0 <br>
10.10.10.0 <br>
30.30.30.0

# Set Neighbour Routing RIP
Router 1 (CR) <br>
Tambahkan neighbour: <br>
10.10.10.2 <br>
20.20.20.2

Router 2 (KJ) <br>
Tambahkan neighbour: <br>
20.20.20.1 <br>
30.30.30.1

Router 3 (KHI) <br>
Tambahkan neighbour: <br>
10.10.10.1 <br> 
30.30.30.2