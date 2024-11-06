# Set ip setiap router
Router 1 (CR)
Ethernet 2: 192.168.30.1/24
Ethernet 3: 10.10.10.1
Ethernet 4: 20.20.20.1

Router 2 (KJ)
Ethernet 2: 192.168.10.1/24
Ethernet 3: 20.20.20.2
Ethernet 4: 30.30.30.2

Router 3 (KHI)
Ethernet 2: 192.168.20.1/24
Ethernet 3: 10.10.10.2
Ethernet 4: 30.30.30.1

# Lakukan DHCP Server setiap router
Router 1 (CR)
DHCP Server -> Ethernet 2

Router 2 (KJ)
DHCP Server -> Ethernet 2

Router 3 (KHI)
DHCP Server -> Ethernet 2

# Set Interface Routing RIP
Router 1 (CR)
Tambahkan Interface 3 | Receive v1-2 | Send v2
Tambahkan Interface 4 | Receive v1-2 | Send V2

Router 2 (KJ)
Tambahkan Interface 3 | Receive v1-2 | Send v2
Tambahkan Interface 4 | Receive v1-2 | Send V2

Router 3 (KHI)
Tambahkan Interface 3 | Receive v1-2 | Send v2
Tambahkan Interface 4 | Receive v1-2 | Send V2

# Set Network Routing RIP
Router 1 (CR)
Tambahkan network:
192.168.30.0
10.10.10.0
20.20.20.0

Router 2 (KJ)
Tambahkan network:
192.168.10.0
20.20.20.0
30.30.30.0

Router 3 (KHI)
Tambahkan network:
192.168.20.0
10.10.10.0
30.30.30.0
