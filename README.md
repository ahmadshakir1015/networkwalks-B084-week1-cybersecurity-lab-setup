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
