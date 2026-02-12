# Creating our Virtual Environment
This section involves the implmentation of the virutal machines, as well as the configuring of them for our Active Directory environment. This lab also serves as a chance for me to fill in knowledge gaps about navigating the Windows and Linux filesystems.

# Table of Contents
- [Hypervisor Setup](#Hypervisor-Setup)
- [Setting up Windows Client](#Setting-up-Windows-Client)
- [Setting up Ubuntu Client]


# Hypervisor Setup
* For this lab, I used VMware
* For more details about my installation of the hypervisor, check my Attack & Defend [project](https://github.com/VincentLindsay/Security-Analysis-Projects/tree/main/Attack%20%26%20Defend%20lab#Setting-up-VirtualBox)

# Setting up Windows 11 Machine
* This Client will utilize a Windows 11 Enterprise retrieved from Microsoft's evaluation [center](https://www.microsoft.com/en-us/evalcenter)
* Under the Windows drop-down menu, I selected Windows 11 enterprise, and selected the ISO for the evaluation edition
<img width="1538" height="975" alt="image" src="https://github.com/user-attachments/assets/3c877199-d80e-44af-aee0-a63f1b574ec5" />
* For these boxes, I entered dummy information
* Once the information is entered I chose the 64-bit download for English(United States)
<img width="1013" height="203" alt="image" src="https://github.com/user-attachments/assets/e7cbed9f-2b46-46d3-9962-60256b63b560" />

* Now that the ISO is downloaded, I can now create a new virtual machine
* I chose a custom installation, and named the machine **Windows AD Client**

* Since Windows 11 does require TPM to be enabled, I enabled it to only be for the necessary files on VMware
<img width="496" height="535" alt="image" src="https://github.com/user-attachments/assets/36eeeaf4-79dc-4ea1-9d42-a0ba2c8bb614" />
<img width="495" height="536" alt="image" src="https://github.com/user-attachments/assets/0b8a4000-f485-4813-ac24-93fb9cbb721f" />

* I did not enable secure boot, and kept the Firmware type to be UEFI
* I allocated 4 CPU cores, 8 GB of RAM, and 80 GB of storage for this VM
* Once the VM is booted up, follow the installation instructions
* Now that Windows is successfully booted, follow the setup instructions
* Once you reach the sign in options page, choose the Domain join instead option
<img width="397" height="442" alt="image" src="https://github.com/user-attachments/assets/580fbcb8-f5e0-42a3-8804-8e052f5f44bd" />

* You can treat it like a local Windows account, and for the username I used my first name
* Create a password, and make answers to the security questions
* I selected no to all of the privacy settings
* Here is the homescreen of a successful Windows 11 Enterprise installation:
<img width="1022" height="768" alt="image" src="https://github.com/user-attachments/assets/79444eff-8e0c-4a43-a0ee-4b9acbf3beae" />





