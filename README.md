# Network and Technology Topology-
## Stage 0
### We started the project with Wan-Cloud and Wan-Switch device that were link in GNS3. 
![image](https://github.com/cmedjo2/network-/assets/130260893/e11fb5a4-5da3-4a54-95a9-91e6bafc125a)
The devices we used for this project were the Wan-Cloud, Wan-Switch, FortiGate, DMZ-Switch, Lan-Switch, Windows 10 and 2012r2, and Unbuntu.

## Stage 1
### Build a network infrastructure for a small business environment.
1. From the Wan-Cloud and Wan-Switch, Add a Fortinet firewall, two Ethernet switches, and a Win10 workstation to the lab workspace.
2. Then, link WAN ports on the firewall to the WAN-SWITCH.
  Link the LAN port on the firewall to the LAN-SWITCH.
  Link the DMZ port on the firewall to the DMZ-SWITCH.
  Link the Win10 workstation to the LAN-SWITCH.
![image](https://github.com/cmedjo2/network-/assets/130260893/f709057a-6d0e-4445-92a6-1480f936e0c2)
3. Start the Firewall on GNS3, then right-click it to select console, and wait a few minutes for setup. Once setup is complete the login screen will pop up. 
4. log in to the console with username: admin then click enter for password and type new password. 
![image](https://github.com/cmedjo2/network-/assets/130260893/57dca260-e337-4c01-9bd2-8f87b1f4da13)
5. configure the LAN interface; this will allow you to access the Firewall GUI from devices on the LAN.
![image](https://github.com/cmedjo2/network-/assets/130260893/e874e04a-f46f-4a34-8473-a3f5d689a84e)
  To verify the configuration type, *show sys int port2*
6. configure the DHCP server for the LAN interface. Enabling the DHCP server on the LAN interface eliminates the need to configure each network host individually.
7. start Win 10 then double click it open.
8. Log in to Win 10, then check network settings.
   Verify the Win 10 workstation has leased a DHCP address from the LAN network.
9. Test network connectivity by pinging LAN, WAN, and Google.
    Only LAN will respond, WAN, and Google will fail as the server has yet to learn their MAC address.
10. from WIN 10 open GUI and configure the network interfaces, enable DNS, configurre the firewall system on DNS, configure DNS, create service object, configure firewall rules, then backup the firewall config.
11.  ![image](https://github.com/cmedjo2/network-/assets/130260893/aeaca252-c782-42cf-aec0-2218b460719d)

## Stage 2
### Build a Windows Domain for the small business environment 
      client request the Domain name to be: Widgest.localdomain
Set up the topology for this station, by adding window 2012r2
![image](https://github.com/cmedjo2/network-/assets/130260893/3698029a-0a2c-4d1a-9ce8-8784a97e0308)
