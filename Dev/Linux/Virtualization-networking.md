
- **DHCP** (Dynamic Host Configuration Protocol) 
	- Asigns Ip addresses.
- **DNS** (Domain Name System) 
	- Translates domains into IP addresses
- **NAT** (Network Address Translation) 
	- Allows multiple devices to share a single public IP.
	- Enables vms to access external networks. 
- **vNIC** (Virtual Network Interface Card)
	- It's used by vms to connect to virtual networks.
- Virtual bridge
	- connects vms to host network.
- dnsmasq
	- service that provides DHCP server and DNS forwarder.

### Diagram

```
Host (Physical Machine)
    |
    v
Operating System (Linux)
    |
    v
KVM (Kernel-based Virtual Machine)
    |
    v
libvirt
    |
    +
    |
    v
Virtual Machine (VM)
    |
    v
  vNIC
    |
    +-------------------------------+
    |                               |
    v                               v
Virtual Bridge / Virtual Switch   Network Services (dnsmasq, NAT)
    |                               |
    v                               v
DHCP, DNS, NAT                    Guest OS
    |                               |
    v                               v
External Network Access        Applications

```
