# Networking

## Routing Protocols and Administrative Distances

In this project, I have configured two PCs, two servers, and various routing protocols to ensure proper connectivity and the best path for network traffic. The Administrative Distance (AD) is used to prioritize these protocols. The lower the AD, the higher the priority.

### Components

1. **PCs (User1 and User2):**  
   - **User1 (PC1)** and **User2 (PC2)** are two personal computers connected to the network. These PCs are used by end-users to access network services such as         email and web browsing.

2. **Servers:**
   - **Email Server:**  
     The email server is configured to handle email communication within the network. It supports sending, receiving, and managing emails for users.
     
   - **DNS Server:**  
     The DNS (Domain Name System) server is set up to resolve domain names to IP addresses. It ensures that user requests to access websites or services are             properly directed to the correct server.

### Administrative Distance Values

- **Static Routing**: AD = 1  
  Static routes are manually configured and have the highest priority. They will be used first if available.

- **EIGRP**: AD = 90  
  Enhanced Interior Gateway Routing Protocol (EIGRP) is used if static routes are unavailable.

- **OSPF**: AD = 110  
  Open Shortest Path First (OSPF) is used if both static routes and EIGRP routes are unavailable.

- **RIP v2**: AD = 120  
  Routing Information Protocol version 2 (RIP v2) is used as a last resort if no other routes are available.
  
This configuration ensures that the network will follow the specified routing path based on the administrative distance of each protocol.
![Screenshot (48)](https://github.com/user-attachments/assets/179cefd4-ad45-49fe-9ee5-ecdf2063f83b)
