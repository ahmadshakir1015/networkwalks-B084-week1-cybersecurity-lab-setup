# networkwalks-B084-week1-cybersecurity-lab-setup
Step-by-step Kali Linux VirtualBox lab setup with NAT Network configuration and practical screenshots.


🪜 Step 1: Check System Requirements
Before installing VirtualBox, check the computer's hardware specifications and whether hardware virtualization is available.
Check:
RAM capacity.
Available storage.
Processor specifications.
Hardware virtualization support.
Screenshot 1: System Requirements
![System Requirements](screenshots/01-system-requirements.png)

🪜 Step 2: Install Oracle VirtualBox
Download VirtualBox from the official website:
Oracle VirtualBox Downloads⁠�
Install the version compatible with your host operating system.
After installation, open VirtualBox and confirm that its main interface appears.
Screenshot 2: VirtualBox Installed
![VirtualBox Installed](screenshots/02-virtualbox-installed.png)

🪜 Step 3: Download Kali Linux
Visit the official Kali Linux download page:
Kali Linux Downloads⁠�
Choose an installation image suitable for a new VirtualBox virtual machine.
Wait for the download to complete.
Screenshot 3: Kali Linux ISO Downloaded
![Kali Linux ISO](screenshots/03-kali-iso-downloaded.png)

🪜 Step 4: Create the Virtual Machine
Open VirtualBox and select New.
Configure:
Name: Kali Linux
Operating system type: Linux
Version: Choose the appropriate 64-bit Debian/Linux option if available.
Select the downloaded Kali Linux ISO when prompted.
Screenshot 4: Virtual Machine Created
![Create Virtual Machine](screenshots/04-create-virtual-machine.png)

🪜 Step 5: Configure Memory and Processors
Allocate memory and processor resources based on the host computer's available capacity.
Avoid allocating so much RAM or CPU capacity that the host operating system becomes unstable.
Record the settings you actually use.
Screenshot 5: Hardware Configuration
![Memory and Processor Configuration](screenshots/05-memory-and-processors.png)

🪜 Step 6: Create the Virtual Hard Disk
Create a virtual hard disk for the Kali Linux installation.
Choose a suitable disk size based on the available storage and the requirements of your installation.
Screenshot 6: Virtual Hard Disk.
![Virtual Hard Disk](screenshots/06-virtual-hard-disk.png)

🪜 Step 7: Install Kali Linux
Start the virtual machine and follow the Kali Linux installation wizard.
Complete the required installation settings and wait for the installation to finish.
After installation, restart the virtual machine and log in.
Screenshot 7: Kali Linux Installation
![Kali Linux Installation](screenshots/07-kali-installation.png)

🪜 Step 8: Create the NAT Network
Open VirtualBox's network configuration interface.
In VirtualBox versions that provide the NAT Network manager, navigate to:
File - Tools - Network Manager - NAT Networks
The exact menu names may vary by version.
Create a new NAT Network with these settings:
Setting
Value
Network name
Kali-NAT
Network IPv4 prefix
10.0.0.0/24
Network mode
NAT Network
DHCP
Enabled, if automatic IP assignment is required
Apply or save the settings.
Screenshot 8: NAT Network Created
![NAT Network Configuration](screenshots/08-nat-network-created.png)

🪜 Step 9: Connect Kali Linux to the NAT Network
Open the settings for the Kali Linux virtual machine.
Navigate to:
Settings - Network - Adapter 1
Configure:
Enable Network Adapter: checked.
Attached to: NAT Network.
Name: Kali-NAT.
Save the changes.
Screenshot 9: Network Adapter Configured
![Network Adapter](screenshots/09-network-adapter-configured.png)

🪜 Step 10: Verify the IP Address
Start Kali Linux and open a terminal.
Run:
ip -4 addr

This command displays IPv4 address information for the system's network interfaces.
Find the active network interface and record the IPv4 address assigned to it.
Screenshot 10: Kali Linux IP Address
![Kali IP Address](screenshots/10-kali-ip-address.png)

🪜 Step 11: Test Network Connectivity
First, check the network interface and its address.
Then test connectivity to a public IP address:
ping -c 4 1.1.1.1
This sends four ICMP echo requests to the destination.
If that succeeds, test DNS resolution:
ping -c 4 example.com
the first test succeeds but the second fails, investigate DNS configuration.
Some networks block ICMP traffic, so a failed ping does not necessarily mean the entire network is unavailable.
Screenshot 11: Network Connectivity Test
![Network Connectivity](screenshots/11-network-connectivity.png)


🧠 What I Learned
Through this practical exercise, I aim to understand:
How to create and manage a virtual machine.
How to install Kali Linux in VirtualBox.
How to configure a NAT Network.
The meaning of an IPv4 subnet and subnet mask.
How to inspect network interfaces in Linux.
How to troubleshoot basic network connectivity.
🏁 Conclusion
This project documents the setup of a Kali Linux virtual machine using Oracle VirtualBox, with a NAT Network configured for the 10.0.0.0/24 subnet.
The accompanying screenshots and test results provide evidence of each stage of the practical exercise.
📚 References
Kali Linux Official Website⁠�
VirtualBox Official Website⁠�

