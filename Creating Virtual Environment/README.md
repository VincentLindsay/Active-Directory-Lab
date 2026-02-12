# Creating our Virtual Environment
This section involves the implmentation of the virtual machines, as well as the configuring of them for our Active Directory environment. This lab will involve the development of several virtual machines, the machines are as follows:
* Windows 11 Enterprise
* Windows Server 2022
* Ubuntu Desktop Linux (Version 24.04)

# Table of Contents
- [Hypervisor Setup](#Hypervisor-Setup)
- [Setting up Windows Client](#Setting-up-Windows-Client)
- [Setting up Ubuntu Client](#Setting-up-Ubuntu-Client)


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

# Setting up Ubuntu Client
* To download the Ubuntu ISO, navigate to Ubuntu's download page for their desktop (iteration)[https://ubuntu.com/download/desktop]
<img width="842" height="517" alt="image" src="https://github.com/user-attachments/assets/2568ff16-81f7-487e-8953-bd984570117a" />
* You do not have to sign up for the newsletter for the download to continue, it will happen automatically
* Once the ISO was downloaded, I began the process on creating a VM for Ubuntu
* VMware has a feature known as easy install that is similar to the unattended installation feature on Virtual Box. For this lab I did not use this feature, and completed the setup manually
* For the VM, I committed 6 GB of RAM, 75 GB of storage, and 2 processors
* Since the manual configuration of the VM does not involve the addition of the ISO, I added the Ubuntu ISO after the configuration of the VM
<img width="885" height="911" alt="image" src="https://github.com/user-attachments/assets/fc5c0d55-58e0-4491-b480-9267a67f3e7e" />






