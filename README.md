# Installing Red Hat Enterprise Linux (RHEL) on VMware

## Introduction to VMware
VMware is a powerful virtualization software that allows you to create and run multiple virtual machines (VMs) on a single physical computer. Each virtual machine operates as a fully functional computer, complete with its own operating system, applications, and resources. This makes VMware an ideal tool for testing, development, and learning environments.

---

### Key Features of VMware:
- **Cross-Platform Support**: Run multiple operating systems (Linux, Windows, macOS) on the same machine.
- **Resource Allocation**: Easily allocate CPU, memory, and storage to VMs.
- **Snapshot Functionality**: Save the state of a VM and revert to it later if needed.
- **Networking Capabilities**: Create isolated or shared networks for VMs.
- **Ease of Use**: User-friendly interface for creating and managing virtual machines.

---
This guide will help you install Red Hat Enterprise Linux (RHEL) in a VMware virtual machine.
---

## Prerequisites

- **VMware Software**: Install VMware Workstation Pro or VMware Player on your host machine.
- **RHEL ISO File**: Obtain the RHEL installation ISO file (e.g., `RHEL-9.4-x86_64-dvd.iso`).
  - Download it from [Red Hat's official website](https://access.redhat.com/).
  - You may need an active Red Hat subscription to access the ISO.
- **System Requirements**:
  - Minimum 2 GB RAM (4 GB recommended)
  - At least 20 GB of disk space for the VM
  - 2 CPU cores

---

## Step-by-Step Installation
1. **Open VMware**  
![Screenshot from 2024-11-27 11-39-48](https://github.com/user-attachments/assets/52034534-9ef1-4b53-ab9c-53ef925bcbd8)

2. **Click on "Create a New Virtual Machine"** 
![Screenshot from 2024-11-27 11-41-36](https://github.com/user-attachments/assets/9313e8e7-502e-42c7-85cc-58c836b43a0a)

3. **Choose the type of configuration**:  
   - Select **Typical** and click **Next**. 
![Screenshot from 2024-11-27 11-42-12](https://github.com/user-attachments/assets/e151defb-4c0c-4660-a832-b39149d4cc0c)

4. **Select "I will install the operating system later"** and click **Next**.  
![Screenshot from 2024-11-27 11-43-24](https://github.com/user-attachments/assets/0f10fb62-1d7d-4bfa-9259-41b02e835f22)

5. **Select the Guest Operating System**:  
   - Choose **Linux**.  
   - Select the appropriate version (e.g., RHEL).  
   - Click **Next**.

![Screenshot from 2024-11-27 11-44-29](https://github.com/user-attachments/assets/ad3a0be0-d83d-45a7-a02e-403c00e1abf4)
![Screenshot from 2024-11-27 11-44-20](https://github.com/user-attachments/assets/36dfbf10-c0a0-4248-8951-70e8b4741c18)

6. **Name your virtual machine**:  
   - Enter a name for the virtual machine and click **Next**
![Screenshot from 2024-11-27 11-45-16](https://github.com/user-attachments/assets/3b04c985-5b0b-48c4-833c-a09c63eb205c)

7. **Choose specific disk capacity**:  
   - Set a disk size (e.g., 20 GB) and click **Next**. 
![Screenshot from 2024-11-27 11-45-33](https://github.com/user-attachments/assets/ceadbb86-89e8-425c-8a62-30470ee948cb)

8. **Finish VM creation**:  
   - Once the VM is created, go to **Edit Virtual Machine Settings**.
![Screenshot from 2024-11-27 11-47-49](https://github.com/user-attachments/assets/37c85487-1fad-41aa-943a-faa69c8da4e4)

9. **Configure the CD/DVD drive**:  
   - Select **CD/DVD (SATA)**.  
   - Choose the ISO image of RHEL from your computer. 
![Screenshot from 2024-11-27 11-47-03](https://github.com/user-attachments/assets/1e05dcb1-fd33-4ebf-8b66-6cab94f193c3)

10. **Configure the network adapter**:  
    - Set the network connection to **Bridged**.
![Screenshot from 2024-11-27 11-47-09](https://github.com/user-attachments/assets/2f2eab63-4743-4318-96f4-4fe4b7189570)

11. **Turn on the virtual machine**:  
    - Start the VM and begin the RHEL installation.  
    - Select **Install Red Hat Enterprise Linux**. If you want to test the ISO, select the second option.  
![Screenshot from 2024-11-27 11-48-54](https://github.com/user-attachments/assets/b30c19f0-11a9-4e25-b6fa-fd8d7ec811af)

12. **Select language**:  
    - Choose your preferred language and click **Continue**. 
![Screenshot from 2024-11-27 11-51-05](https://github.com/user-attachments/assets/a7d255e2-0f21-4ca7-a5f5-5e8e978ad2e1)

13. **Configure installation destination**:  
    - In the new screen, select **Installation Destination**.  
![Screenshot from 2024-11-27 11-52-32](https://github.com/user-attachments/assets/0fd4c87c-c0d3-412c-bdb8-d7f98143b9e8)
    - Choose **VMware Virtual NVMe Disk** and click **Done**.  
![Screenshot from 2024-11-27 11-52-53](https://github.com/user-attachments/assets/4d4ba78f-eeb6-4128-bf67-38cae3ab6c42)

14. **Set up users**:  
    - **Root Password**: Create a strong password for the root user.  
![Screenshot from 2024-11-27 11-53-28](https://github.com/user-attachments/assets/6dfe11fa-16c7-440f-b581-124d49d84e66)
![Screenshot from 2024-11-27 11-53-49](https://github.com/user-attachments/assets/3f0368b2-5917-4236-8146-d53ff4ca7fa6)
   - **User Creation**: Create a regular user for daily use. 
![Screenshot from 2024-11-27 11-54-22](https://github.com/user-attachments/assets/207926e4-42d6-4ca0-badf-58a582879d6a)
![Screenshot from 2024-11-27 11-54-41](https://github.com/user-attachments/assets/7330aaec-addb-4427-abd5-7a918509d5f8)

15. **Begin installation**:  
    - Once all configurations are complete, click **Begin Installation**.  
    - The installation will take some time.
![Screenshot from 2024-11-27 11-55-05](https://github.com/user-attachments/assets/f3a92f76-f0f2-4218-a872-1a6375acd2a7)

16. **After installation**:  
    - A login screen will appear.  
    - To log in as the root user, click **Not Listed**, type `root`, and enter the password.  
![Screenshot from 2024-11-27 13-09-11](https://github.com/user-attachments/assets/05a18cfa-1b06-480c-a407-07b3016542b1)
![Screenshot from 2024-11-27 11-58-43](https://github.com/user-attachments/assets/7a6d58cc-e5c5-4c1c-9cf9-2d32b4d3053a)
![Screenshot from 2024-11-27 11-58-56](https://github.com/user-attachments/assets/2544d281-3eba-4450-ba76-235c2d10f3bf)
