# Home-Security-Lab
The aim of this project was to set up a home security lab equipped with a virtualized system running pfSense and Kali Linux, and to test the system using Metasploitable 2. The steps below were taken:

•	Install and configure VirtualBox

•	Install and configure pfSense	

•	Install and configure Kali Linux

•	Install and configure Metasploitable2

•	Confirming connection between MS2 and Kali

# **Install and configure VirtualBox**
![image](https://github.com/user-attachments/assets/6575376c-19e0-4c1d-82cb-dafb87c154c2)
# **Install and configure pfSense**
Insert name and configure system using Linux
![image](https://github.com/user-attachments/assets/388a78d8-c752-4d5f-a29e-7ce47f89f1d6)

Continue to select the default settings, including the keeping the disk size at 8 GB
![image](https://github.com/user-attachments/assets/136bce10-6620-4375-9e63-2c3ae99b6106)

This will create the VM, under [Optical Drive] load the pfSense iso file
![image](https://github.com/user-attachments/assets/456ef4fe-9e98-43f2-8d9c-2b6a7acfd987)

Click on Network -> Adapter 2 -> Attached to Internal Network -> click OK
![image](https://github.com/user-attachments/assets/9515d496-e282-4a07-8e7d-9a6b10dffde4)

This will start installing pfSense. Select the default values
![image](https://github.com/user-attachments/assets/a7f20680-d86d-47a4-9c5a-ece463318e7d)

Click Start VM VirtualBox, this displays the menu below. Do the following at the Enter an option prompt: 2 then 2; enter the new LAN IPv4 address – 10.13.37.1; subnet bit count will be 24; don’t specify IPv4 upstream gateway address, press <ENTER>; disable IPv6; select Yest to enable DHCP server; start range for IPv4 client address range will be 10.13.37.100 to 10.13.37.200; click Yes to using HTTP as the protocol and press <ENTER> again.
![image](https://github.com/user-attachments/assets/fa3bf2a1-3d81-4019-8461-5943187042c3)



