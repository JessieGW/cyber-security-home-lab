## Networking the Lab

### Objective
- Finish Windows 10 setup.
- Verify both VMs boot correctly.
- Configure an isolated Host-Only network between Kali Linux and Windows 10 while maintaining internet access through NAT.
- Troubleshoot Virtualbox networking issues.
- Verify communication between Kali and Windows.

### Finished Windows 10 Install
- Completed Windows Out-of-Box Experience (OOBE)
- Created a local user account.
- Reached the Windows desktop successfully.
  
### Verified Virtual Machines
- Booted Kali Linux
- Booted Windowos 10
- Confirmed both operating systems were working correctly.

### Configuration
- Initial configuration
- Adapter 1: NAT
- Adapter 2: Host-Only
- Host-Only subnet: 192.168.254.1/24

### Troubleshooting
Encountered several networking issues including: 
- VERR_INTNET_FLT_IF_NOT_FOUND
- "Failed to open/create the internal nework"

Troubleshooting steps:
- Deleted and recreated the Virtualbox Host-Only Adapter.
- Verified the Virtualbox networking service.
- Confirmed the virtual cable was connected.
- Verified IPv4 settings.
- Restarted Virtualbox.
- Adjusted Windows Firewall settings to allow ICMP.

### Verification of Connectivity
- Verified IP addresses on both VMs
-- Kali: 192.168.254.3
-- Windows: 192.168.254.4
  
- Successfully pinged between Kali and Windows.
- Both systems responded successfully to ICMP (ping).
-- Kali ---> Windows
-- Windows ---> Kali
- Confirmed internet connectivity through NAT.

### Skills Demonstrated
- Virtualbox administration
- Windows 10 deployment
- Kali Linux administration
- Virtual networking
- Host-Only networking
- VM troubleshooting
- IPv4 addressing
- Firewall troubleshooting
- Network connectivity testing
- Basic troubleshooting methodology.

### Reflection
This lab reinforced the importance of systematic troubleshooting. After resolving Virtualbox host-only networking and firewall issues, I successfully established communication between my Kali Linux and Windows 10 virtual machines, creating the foundation for future penetration testing and network analysis exercises.
