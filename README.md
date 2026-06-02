# Introduction

Routing Information Protocol (RIP) is a dynamic routing protocol used in computer networks to exchange routing information between routers automatically. RIP helps routers determine the best path for forwarding packets using hop count as the routing metric.

RIP is one of the simplest routing protocols and is widely used for educational purposes and small networks.

---

# Objective

- To understand the working of RIP
- To configure dynamic routing between routers
- To establish communication between different networks
- To simulate routing using Cisco Packet Tracer
- To observe routing updates and packet flow

---

# Software Requirements

- Cisco Packet Tracer

---

# Devices Used

| Device | Quantity |
|---|---|
| PC | 2 |
| Switch | 2 |
| Router | 2 |
| Copper Straight Through Cable | Multiple |
| Serial DCE Cable | 1 |

---

# Network Topology

<img width="1024" height="597" alt="image" src="https://github.com/user-attachments/assets/aa052840-2378-4e5a-94f8-f205b1274296" />


# IP Address Configuration

| Device | Interface | IP Address | Subnet Mask |
|---|---|---|---|
| PC0 | FastEthernet0 | 192.168.1.2 | 255.255.255.0 |
| Router0 | FastEthernet0/0 | 192.168.1.1 | 255.255.255.0 |
| Router0 | Serial0/0/0 | 10.0.0.1 | 255.255.255.252 |
| Router1 | Serial0/0/0 | 10.0.0.2 | 255.255.255.252 |
| Router1 | FastEthernet0/0 | 192.168.2.1 | 255.255.255.0 |
| PC1 | FastEthernet0 | 192.168.2.2 | 255.255.255.0 |


# Theory of RIP

Routing Information Protocol (RIP) is a distance-vector routing protocol that uses hop count to find the best path between networks.
<img width="1024" height="394" alt="image" src="https://github.com/user-attachments/assets/a23e00bf-a477-4398-8e53-2c9a07472619" />


## Features of RIP

- Distance-vector routing protocol
- Uses hop count as metric
- Maximum hop count is 15
- Routing updates every 30 seconds
- Uses UDP port 520
- Easy to configure

---
## NETWORK DIAGRAM:
<img width="1559" height="819" alt="image" src="https://github.com/user-attachments/assets/81ae0fba-56d2-409c-818f-382cb6a7be52" />


# Working Principle of RIP

<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/eb53bf9c-c60b-4f81-a1cd-92decf274d77" />


---
# Procedure

```
STEP 1: Open a Packet Tracer Software.
STEP 2: Drag two 2900 Switches, two Cisco 1800 Routers, four PC Terminals from tool barand drop it in work area.
STEP 3: Connect all the PC Terminals and Routers through Switches as shown in the networkdiagram using CAT 6 Patch cables.
STEP 4: Configure IP address and Gateway in all PC Terminals.
STEP 5: Configure ROUTER0 and restart ROUTER0.
STEP 6: Configure ROUTER1 and restart ROUTER1.
STEP 7: Verify the connectivity between PC Terminals in different networks using Pingcommand.
After This follow the given procedure
1. Assign IP Addresses to PCs
•	For each PC, go to Desktop > IP Configuration and assign:
o PC0: 192.168.1.2, Subnet Mask: 255.255.255.0, Gateway: 192.168.1.1
o PC1: 192.168.1.3, Subnet Mask: 255.255.255.0, Gateway: 192.168.1.1
o PC2: 192.168.2.2, Subnet Mask: 255.255.255.0, Gateway: 192.168.2.1
o PC3: 192.168.3.2, Subnet Mask: 255.255.255.0, Gateway: 192.168.3.1
o PC4: 192.168.4.2, Subnet Mask: 255.255.255.0, Gateway: 192.168.4.1
o PC5: 192.168.4.3, Subnet Mask: 255.255.255.0, Gateway: 192.168.4.1
```

# PC Configuration

## PC0

```text
IP Address : 192.168.1.2
Subnet Mask: 255.255.255.0
Default Gateway: 192.168.1.1
```
<img width="724" height="651" alt="image" src="https://github.com/user-attachments/assets/5bb595f0-b72e-4bcb-86da-8417c7942c8e" />

---

## PC1

```text
IP Address : 192.168.2.2
Subnet Mask: 255.255.255.0
Default Gateway: 192.168.2.1
```
<img width="564" height="582" alt="image" src="https://github.com/user-attachments/assets/a58662c7-9930-48c8-a81a-2a70185415b1" />

---

# Expected Output

<img width="869" height="781" alt="image" src="https://github.com/user-attachments/assets/a5441c53-bf21-4896-9feb-70389c96155d" />


---

# Advantages of RIP

1. Easy to configure
2. Automatic route updates
3. Suitable for small networks
4. Simple routing mechanism
5. Low configuration complexity

---

# Disadvantages of RIP

1. Slow convergence
2. Maximum hop count is 15
3. Not suitable for large networks
4. Generates periodic traffic
5. Less efficient than modern protocols

---

# Applications of RIP

1. Small office networks
2. Educational simulations
3. Basic routing implementation
4. LAN routing
5. Academic networking experiments

---

# Real-Time Scenario of RIP

Consider two branch offices connected using routers.

- Office A network: 192.168.1.0/24
- Office B network: 192.168.2.0/24

RIP automatically exchanges routing information between routers and allows communication between devices in both offices.

---

# Conclusion

Thus, the RIP simulation was successfully implemented using Cisco Packet Tracer. Dynamic routing was established between two different networks using RIP. Routers exchanged routing information automatically and successfully forwarded packets between networks.

---

# Viva Questions and Answers

## 1. What is RIP?

RIP stands for Routing Information Protocol.

---

## 2. Which metric is used by RIP?

Hop count.

---

## 3. What is the maximum hop count in RIP?

15 hops.

---

## 4. Which port does RIP use?

UDP port 520.

---

## 5. Which type of routing protocol is RIP?

Distance-vector routing protocol.

---

## 6. Why is RIP called dynamic routing?

Because routers exchange routing information automatically.

---

## 7. Which software is used for this simulation?

Cisco Packet Tracer.

---

## 8. What is the purpose of RIP?

To determine the best path between networks automatically.

---

## 9. What happens when hop count exceeds 15?

Destination becomes unreachable.

---

## 10. Which command enables RIP?

```bash
router rip
```

---

# References

1. Cisco Networking Academy

2. Cisco Packet Tracer Documentation

3. Data Communications and Networking — Behrouz A. Forouzan

4. Computer Networks — Andrew S. Tanenbaum

5. Routing and Switching Essentials — Cisco
