# Powershell Automation
![image](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/efae0558-bebb-4065-8e64-4698b5e832ef)

<h1>Automating basic day-to-day tasks using PowerShell on Virtual Machines deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of scripts via Powershell in order to streamline the process of starting and ending a typical work day for an office employee. Instead of spending valuable company time on opening and closing applications, we can consolidate all those actions into a couple simple clicks in order to save time and effort. This could be especially useful for less tech savvy individuals who are not used to locating and opening/closing applications on their PC. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment Steps</h2>

- Creating and deploying a Virutal Machine to set up our work environment
- Downloading several applications via the internet
- Writing our scrpit for opening/closing applications, then importing them into powershell

<h2>Configuration Steps</h2>

First, we will use Microsoft Azure to set up a Virtual Machine for us to use as a test environment. Be sure to copy the Public IP address on the top right, as this will be needed to remote into the virtual machine in the next step
![vm setup](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/1bee74fa-1e03-45fe-9b1b-b3471de6a535)

Paste the public IP address of the Vitual Machine into the search bar and log into the VM with your username and password.
![remote](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/e2583a61-0778-4633-b30a-42cfc0888f3e)

Next, once logged in, use the the default internet browser to search for, download and install a few applications which will be the basis for our scripts. For this demonstration, I've decided to download OBS, Microsoft Teams, and VLC for this demonstration, as these may be some common applications used in a day-to-day office setting, however most any application could be used for this script.

![obs](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/78be3b9e-d807-4479-bab8-743ef737aaec)

![teams](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/dacefeec-e105-40cd-9d48-6e71ea49839c)

![vlc](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/8ed3bb82-6aad-4fa2-b260-c795e3bd7207)



