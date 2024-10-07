# Create Ubuntu 24.04 server LTS Virtual Machine on VirtualBox

### 1. Description

This project aims to demonstrate how to create a Ubuntu 24.04 Server Virtual Machine on Oracle VirtualBox.

### 2. Objectives

- Set up a VM with Ubuntu Operating system.

### 3. Tools and Technologies Used

- **VirtualBox**: Used for creating virtual machines for the lab environment.
- **Ubuntu Server 24.04 LTS**: Used as a monitored system.


### 4. Installation Steps
   
First, we need to download the ISO file from the Ubuntu official webpage, so we go <a href="https://ubuntu.com/download/server">here</a> and click the button shown below to download the ISO.

<p align="center">
  <img src="https://github.com/user-attachments/assets/a2ba2766-e299-41df-858f-c4f99ea56dbe" alt="Download the Ubuntu ISO" width="500"/>
</p>

   - **4.1. Create the VM on VirtualBox**

Open VirtualBox, then click Machine => New, then folow the steps indicated in the image below.

<p align="center">
<img width="520" alt="VM creation on VirtualBox" src="https://github.com/user-attachments/assets/c117c240-884e-4d46-82c9-d95eeee406e6">
</p>

   - **4.2. Connect the VM to the correct interface**

Before starting the machine, choose the NAT Network created <a href="https://github.com/Muhate/Setting-Up-VirtualBox/blob/main/README.md">here</a>. For that, just folow the steps indicated in the image below. By the end start the machine.

<p align="center">
<img width="520" alt="VM creation on VirtualBox" src="https://github.com/user-attachments/assets/0d59c54d-125a-41db-bff1-36347506704d">
</p>

   - **4.2. Configure the VM**

After starting the VM, let's configure it. When you're prompted with the screen below, choose ***Try or Install Ubuntu Server**. If nothing is happening, try to click any place inside the black screen.

<p align="center">
<img width="520" alt="Start the installation" src="https://github.com/user-attachments/assets/42348668-1753-4918-ac4e-e9cf912b0787">
</p>

Choose the language for the installation process and hit "ENTER"

<p align="center">
<img width="520" alt="Language Selection" src="https://github.com/user-attachments/assets/a561141c-c2fb-4a83-a1c6-fbdbe730a715">
</p>

Select the keyboard of your preference or that you are using, select **"Done"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Language Selection" src="https://github.com/user-attachments/assets/471f2b49-f3af-485b-ad74-1c74f01bb509">
</p>

Choose the type of installation, in this lab we choose **"Ubuntu Server"**, select **"Done"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Installation Selection" src="https://github.com/user-attachments/assets/99ea9b69-118f-47af-9a83-d4613dad51db">
</p>

Configure the network, select **"Done"** and hit **"ENTER"**. You can skip this step or let it be configured dynamically. Here it was configured manually.

<p align="center">
<img width="520" alt="Network configuration" src="https://github.com/user-attachments/assets/fc4a8ba8-29df-4f17-965b-c06d0bd4335b">
</p>

No proxy is required, so just select **"Done"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Proxy configuration" src="https://github.com/user-attachments/assets/33d5c4c2-be08-4e6d-b5b8-4cc249d2b17e">
</p>

Nothing to change, keep the default Ubuntu mirror, select **"Done"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Mirror configuration" src="https://github.com/user-attachments/assets/fe1d235d-d369-44c1-b2fd-b4c0baa117a6">
</p>

Select **"Continue"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Mirror check" src="https://github.com/user-attachments/assets/0c569dbe-6f0c-4b3f-884c-32e39c79068c">
</p>

The default configurations for the storage are fine, just select **"Done"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Storage configuration" src="https://github.com/user-attachments/assets/9d9ce1e3-579f-4629-9832-585d100170f3">
</p>

Review the storage configurations, if they are good select **"Done"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Storage configuration review" src="https://github.com/user-attachments/assets/59d9f252-8ba4-44cf-bd55-aef1b7f004a4">
</p>

Read the warning and if you are confortable with the storage configurations, just select **"Continue"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Storage configuration warning" src="https://github.com/user-attachments/assets/a6aa04db-b0d5-4ba7-a5d6-8f5e9b2a6e80">
</p>

Configure your profile accordingly, select **"Done"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Profile configuration" src="https://github.com/user-attachments/assets/90fa6dac-64df-45e3-ac08-fec0b46e10b7">
</p>

Skip the Ubuntu Pro installation, select **"Continue"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Ubuntu Pro" src="https://github.com/user-attachments/assets/94fd94c2-44a2-4099-bba9-06281fc41aea">
</p>

Select to install OpenSSH Server, select **"Done"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Ubuntu Pro" src="https://github.com/user-attachments/assets/1d17e548-a47e-46a6-8a74-afe5c74f6391">
</p>

In the Featured server snaps, just hit **"tab"** to select **"Done"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Featured server snaps" src="https://github.com/user-attachments/assets/ae39f29f-94fc-4c23-905d-44ac27b42a15">
</p>

Let the installation occur and when finished, select **"Reboot now"** and hit **"ENTER"**.

<p align="center">
<img width="520" alt="Installation complete" src="https://github.com/user-attachments/assets/a15abeef-8f2c-454c-9f75-b1c4ae6473d5">
</p>

When prompted with the screen below, just hit **"ENTER"**.

<p align="center">
<img width="520" alt="enter to reboot" src="https://github.com/user-attachments/assets/023b529e-592d-4104-9ee9-ae3347916b9d">
</p>

### 5. **Conclusion**
   - This project successfully demonstrated the creation of a VM on VirtualBox with Ubuntu 24.04 Server operating system.

### 12. **Contact Information**
   - **Name**: Rogério Muhate
   - **Email**: rbmuhate@gmail.com
   - **LinkedIn**: [LinkedIn Profile](https://www.linkedin.com/in/rmuhate)



