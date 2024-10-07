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

### 5. Installation Steps
   - **5.1. Setting Up VirtualBox**

For setting up VirtualBox, refer to <a href="https://github.com/Muhate/Setting-Up-VirtualBox">this guide</a>
<br>
<br>
   
   - **5.2: Setting Up Windows 2022 on VirtualBox**

For setting up Windows 2022 on VirtualBox, refer to <a href="https://github.com/Muhate/Install-Windows-on-VirtualBox">this guide</a>
<br>
<br>

   - **5.3: Setting Up Ubuntu Server 24.04.LTS on VirtualBox**

For setting up Ubuntu Server on VirtualBox, refer to <a href="https://github.com/Muhate/Install-Ubuntu-on-VirtualBox">this guide</a>
<br>
<br>

   - **5.3: Setting Up Wazuh Manager on Ubuntu Server 24.04 LTS**

     - Update the package manager:
       ```
       sudo apt update && sudo apt upgrade -y && sudo reboot
       ```
     - Install Wazuh Manager:
       ```
       curl -s https://packages.wazuh.com/4.x/ubuntu/KEY.gpg | sudo apt-key add -
       echo "deb http://packages.wazuh.com/4.x/ubuntu/ focal main" | sudo tee /etc/apt/sources.list.d/wazuh.list
       sudo apt-get update
       sudo apt-get install wazuh-manager
       ```

   - **Step 3: Configuring Wazuh**
     - Modify the configuration file (`/var/ossec/etc/ossec.conf`) to set up agents and alerts.
     - Restart Wazuh Manager:
       ```bash
       sudo systemctl restart wazuh-manager
       ```

   - **Step 4: Installing Elasticsearch and Kibana**
     - Follow similar steps to install and configure Elasticsearch and Kibana.

### 5. **Generating Test Data**
   - **Kali Linux Testing**: 
     - Execute various tests to generate logs (e.g., using Metasploit, Nmap).
     - Sample command to generate logs:
       ```bash
       nmap -sS -p 1-65535 <target_ip>
       ```

### 6. **Results and Analysis**
   - **Data Visualization**: 
     - Showcase screenshots of dashboards in Kibana that display security events, logs, and alerts.
   - **Alerts Configuration**:
     - Explain how alerts were configured in Wazuh and provide examples of alerts generated during testing.

### 7. **Challenges and Solutions**
   - **Challenge**: Difficulty in integrating Wazuh with Elastic Stack.
     - **Solution**: Consulted official documentation and community forums, which helped resolve configuration issues.

### 8. **Lessons Learned**
   - Gained hands-on experience in setting up a complete SIEM solution.
   - Improved understanding of log analysis and incident response workflows.

### 9. **Future Improvements**
   - Plan to integrate additional data sources (e.g., firewalls, web servers).
   - Explore automated incident response mechanisms using Wazuh.

### 10. **Conclusion**
   - This project successfully demonstrated the deployment of Wazuh in a lab environment, providing valuable insights into security monitoring and log analysis.

### 11. **Links and References**
   - [GitHub Repository](https://github.com/username/wazuh-lab)
   - [Wazuh Official Documentation](https://wazuh.com/documentation/)
   - [Elastic Stack Documentation](https://www.elastic.co/guide/en/elastic-stack/current/index.html)

### 12. **Contact Information**
   - **Name**: Rogério Muhate
   - **Email**: rbmuhate@gmail.com
   - **LinkedIn**: [LinkedIn Profile](https://www.linkedin.com/in/rmuhate)



