# Home-Security-Lab
The aim of this project was to set up a home security lab equipped with a virtualized system running pfSense and Kali Linux, and to test the system using Metasploitable 2. The steps below were taken:

<details>
  <summary><b>Install and configure VirtualBox</b></summary>
  
![image](https://github.com/user-attachments/assets/6575376c-19e0-4c1d-82cb-dafb87c154c2)

</details>

<details>
  <summary><b>Install and configure pfSense</b></summary>

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
</details>

<details>
  <summary><b>Install and configure Kali Linu</b></summary>

Download and install the VirtualBox 64 bit version
![image](https://github.com/user-attachments/assets/419cf587-7665-45f1-bc6d-3f1f3bb4dfa9)

Click on Network

![image](https://github.com/user-attachments/assets/ccdfa49b-8454-4138-83e1-c2218387b086)

Attached to: Internal Network, which will be MyHackNetwork.
![image](https://github.com/user-attachments/assets/2c910aa1-abc8-44f2-95e9-f76da2be548b)

Click on Start Kali

![image](https://github.com/user-attachments/assets/2e5de63c-04f5-4a25-a96a-969cda6e3675)

Open browser and enter 10.13.37.1, which will open the control panel for pfSense. Disable RFC1918 Networks and Block bogon networks
![image](https://github.com/user-attachments/assets/6f9d0311-9824-48f0-a62f-7d776a2166e2)

Reload and the Dashboard below will be displayed
![image](https://github.com/user-attachments/assets/fd7f322d-6ef2-4c61-b7a0-4e531119b7a3)
</details>

<details>
  <summary><b>Install and configure Metasploitable2</b></summary>

![image](https://github.com/user-attachments/assets/33f895e7-8e4c-4f46-a1da-df831032ee84)

![image](https://github.com/user-attachments/assets/33a4c060-646b-4a08-be95-41233b21d561)

Click on Adapter 1 and select the settings below and click OK.
![image](https://github.com/user-attachments/assets/a2ec3647-cfe9-4199-b594-778981654ae6)
</details>

<details>
  <summary><b>Confirming connection between MS2 and Kali</b></summary>

In Kali, run nmap scan by entering nmap 10.13.37.*
![image](https://github.com/user-attachments/assets/e69a710e-e045-41af-8348-abcb9490f9c7)

While in Kali, use browser and enter 10.13.37.102 (the ip of MS2)
![image](https://github.com/user-attachments/assets/c7e4064b-0505-4a1e-845e-0b0e2da8b301)
</details>





