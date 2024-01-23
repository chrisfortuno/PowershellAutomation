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

Next, once logged in, use the the default internet browser to search for, download and install a few applications which will be the basis for our scripts. For this demonstration, I've decided to download OBS, Microsoft Teams, and VLC, as these may be some common applications used in a day-to-day office setting, however most any application could be used for this script.

![obs](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/78be3b9e-d807-4479-bab8-743ef737aaec)

![teams](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/dacefeec-e105-40cd-9d48-6e71ea49839c)

![vlc](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/8ed3bb82-6aad-4fa2-b260-c795e3bd7207)

Afterwards, we will go to the 'Start' button on the bottom left of our PC and type in "Windows Powershell ISE" and open the application. Here, we will write our script which will automate opening these applications. To explain the scripting language, "invoke" is the verb, which tells the script what to do, and "item" is the noun, which tells the computer what it is actually invoking. What comes after is the file path, which tells the script where to look for the application (.exe file) that we want, at which point it will simply open the application as if we were double-clicking it as usual.

![powershell open](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/c33319ae-9fdf-4375-9570-fff7369d4aad)

![powershell script](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/6a9c33f6-4e1e-4d31-a2d0-f5733de8cdc0)

After writing the script as shown, we will go to 'File' and save as 'open applications' in a new folder created on the desktop. This will make the script easily accessible for the user

![file save](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/44de2366-d505-4d46-a82a-9a28485471d9)

Next, we will create a new script, this time for automatically closing the applications. So we will do the same process as before, write the script as shown in the photo and save as 'Close applications' in the desktop folder

![Close applications](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/dfee72a5-ecfc-486b-a206-2662d925818c)

After that, we will go to the the folder containing the Powershell scripts. Here we will go to the 'Open applications' file, right click and select 'Run with Powershell'

![run with powershell](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/8c13383a-d423-4582-a714-b49739410b67)

If done correctly, the script should open VLC, OBS, and Teams all at once

![applications open](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/479601dd-06bb-4cca-b21c-336cde87fc80)

Now, once our hypothetical office worker is done for the day and ready to close down their PC, they can now use the 'Close application' script in the same way as we just did previously. Go to the folder with the powershell scripts, right click 'Close applications' and click 'run with powershell'. Once that is done, all applications open on the PC will close simultaniously. 

![apps closed](https://github.com/chrisfortuno/PowershellAutomation/assets/149267076/e47d686b-8ee4-47b2-a842-a878585baea7)

This simple tutorial demonstrates how Powershell can be used to make simple tasks faster and more streamlined for users who may struggle with locating and logging into their daily applications 















