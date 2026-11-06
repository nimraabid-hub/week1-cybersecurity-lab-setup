Cybersecurity Lab Setup – VirtualBox & Kali Linux

 Project Overview

This project focuses on setting up a controlled cybersecurity testing and learning environment using Oracle VirtualBox and Kali Linux.

The purpose of this lab is to create a virtual environment for practicing cybersecurity concepts, networking, troubleshooting, and future ethical security testing activities.

The lab uses a Kali Linux virtual machine running inside Oracle VirtualBox.

 Objectives

The main objectives of this project are:

- Install and configure Oracle VirtualBox.
- Install Kali Linux as a virtual machine.
- Create and configure a custom NAT Network.
- Configure network connectivity.
- Verify the assigned IP address.
- Configure a shared folder between the host and virtual machine.
- Test internet connectivity.
- Create a virtual machine snapshot.
- Document the complete setup process.

 Tools and Technologies

| Component | Description |
|---|---|
| Host Operating System | Windows |
| Virtualization Platform | Oracle VirtualBox |
| Virtual Machine OS | Kali Linux |
| Virtual Network | NAT Network |
| Network Configuration | IPv4 |
| Testing Tool | Kali Linux Terminal |

 Lab Architecture

The laboratory consists of:

1. Host Computer (Windows)
2. Oracle VirtualBox
3. Kali Linux Virtual Machine
4. Virtual NAT Network
5. Shared Folder

The Kali Linux virtual machine operates inside VirtualBox, providing a separate environment for cybersecurity learning and authorized testing.

Lab Setup Process

 Step 1 – Install Oracle VirtualBox

Download Oracle VirtualBox from its official website and install it on the host computer.

Website: https://www.virtualbox.org/

VirtualBox allows users to create and operate virtual machines.

step 2– Download Kali Linux

Download the official Kali Linux VirtualBox image.

Website: https://www.kali.org/get-kali/

Import the downloaded virtual machine into Oracle VirtualBox.

 Step 3 – Configure Kali Linux Virtual Machine

Configure the virtual machine according to your computer's available resources.

Example configuration:

- Operating System: Kali Linux
- RAM: 2048 MB (adjust according to available memory)
- Processor: 2 CPUs (if supported)
- Network Adapter: NAT Network

 Step 4 – Create a NAT Network

Open VirtualBox Network Manager and create a custom NAT Network.

Example configuration:

- Network Name: CyberLab
- IPv4 Prefix: 10.0.0.0/24
- DHCP: Enabled

A NAT Network allows connected virtual machines to communicate with each other and access the internet through network address translation.

 Step 5 – Configure Network Adapter

Open Kali Linux VM settings.

Navigate to:

Settings → Network → Adapter 1

Configure:

- Enable Network Adapter: Yes
- Attached To: NAT Network
- Name: CyberLab
- Adapter Type: Intel PRO/1000 MT Desktop

Save the settings and start Kali Linux.

 Step 6 – Verify IP Address

Open the Kali Linux terminal and execute:



You can also use:


Check the assigned IPv4 address of the active network interface.

Step 7 – Test Internet Connectivity

Use the following command:

```bash
ping -c 4 8.8.8.8
```

This command sends four packets to test network connectivity.

Successful replies indicate that the VM can reach the destination.

 Step 8 – Configure Shared Folder

Open VirtualBox:

Settings → Shared Folders

Add a folder from the host computer.

Configure the folder name and enable Auto Mount if required.



 Step 9 – Create a VM Snapshot

After completing the initial configuration, create a snapshot of the virtual machine.

Suggested snapshot name:

Week 1 - Clean Lab Setup

A snapshot provides a restore point for future experiments.

 Screenshots and Evidence
 




 What I Learned

Through this project, I gained practical knowledge of:

- Virtualization and virtual machines
- Oracle VirtualBox
- Kali Linux
- NAT Networking
- IPv4 addressing
- Network configuration
- Linux terminal commands
- Internet connectivity testing
- Shared folders
- Virtual machine snapshots
- Basic cybersecurity lab management

Security and Ethical Use

This laboratory is intended for cybersecurity education and authorized testing only.

All security testing must be performed on systems owned by the user or where explicit permission has been granted.

Unauthorized access and testing are not permitted.

Future Improvements

Possible future improvements include:

- Adding another virtual machine as a testing target.
- Learning network scanning.
- Practicing reconnaissance techniques.
- Exploring Kali Linux security tools.
- Performing controlled vulnerability assessments.
- Creating isolated Capture The Flag environments.

Conclusion

This project provides practical experience in creating a cybersecurity lab using Oracle VirtualBox and Kali Linux.

It helps develop an understanding of virtualization, networking, IP addressing, connectivity testing, and basic Linux commands.

The laboratory will serve as a foundation for future cybersecurity learning and ethical security testing.

Author

Name: NIMRA ABID 

GitHub: nimraabid-hub

Project: Cybersecurity Lab Setup – VirtualBox & Kali Linux
