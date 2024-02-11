<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>Actions and Observations</h2>

Step 1: Create a Resource Group and 2 Seperate Virtual Machines using Microsoft Azure. 

![image](https://github.com/Tstewart2408/Azure-Network-Protocols-/assets/158493074/ab821568-3855-46fb-b738-267f2a52a8d9)

Step 2: Connect to your Windows 10 Virtual Machine using Remote Desktop.
![image](https://github.com/Tstewart2408/Azure-Network-Protocols-/assets/158493074/57ca22c5-3330-4f72-9095-0e03abcc9db2)

Step3: Install WireShark onto your Windows 10 Virtual Machine. 

![image](https://github.com/Tstewart2408/Azure-Network-Protocols-/assets/158493074/041b8d82-953a-4cbb-9e0b-42695c8a2f42)

Step 4: Open WireShark and set a filter to show only ICMP traffic. Using the private IP address from Ubuntu VM to ping Windows 10 VM. Observe the ping messages and replies in Wireshark. Use command line or PowerShell in your Windows 10 VM to ping a public website (like www.google.com) and check the traffic in Wireshark.

![image](https://github.com/Tstewart2408/Azure-Network-Protocols-/assets/158493074/d7d60edf-5d2a-4a21-ab07-3cbff05f1d76)

Step 5: After observing ICMP traffic, we will filter WireShark to observe SSH Traffic, DHCP Traffic, DNS Traffic, and RDP Traffic

![image](https://github.com/Tstewart2408/Azure-Network-Protocols-/assets/158493074/54efdcb6-d9b9-49d5-a294-c6f8208d44b2)

![image](https://github.com/Tstewart2408/Azure-Network-Protocols-/assets/158493074/33312add-8fc6-494b-82c6-6a487b36e6b2)

![image](https://github.com/Tstewart2408/Azure-Network-Protocols-/assets/158493074/ab26feb4-9eb8-4574-bddb-61a5311c0cfd)

Step 6: Don't forget to clean up your lab by closing the remote desktop connection, deleting resource group(s) created at the beginning of the lab, and verify resource group deletion.

![image](https://github.com/Tstewart2408/Azure-Network-Protocols-/assets/158493074/573e66e7-813c-4711-a117-2887e679c235)

![image](https://github.com/Tstewart2408/Azure-Network-Protocols-/assets/158493074/08e7d16a-4a85-4c1d-b0f0-319409254fe5)

