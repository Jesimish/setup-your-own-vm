# Create a VM lab
What OS is your VM running? 
    My VM is running Ubuntu
## What challenges did you face while creating your VM? What troubleshooting steps did you take to resolve those challenges and what did you research?
First, my computer showed a "NtCreateFile(\Device\VBoxDrvStub) failed: 0xc000000034" error which I shared in Office Hours on 05/07/25 and Alexandra looked up blog threads and through trial and error, we figured otu that I was not running the VM as an administration.
        
**Steps to correct in the future:**
1. Open Command Prompt as administrator
2. type in net start vboxsup
3. Open VirtualBox as Administrator


The second error I experiences was a black screen after bootup.
        
**Research:** Googled the error and found a Stack Exchange thread that recommended changing the Graphics controller to VBoxVGA.
1. Open VirtualBox Settings
2. Open display
3. Change the Graphics Controller to VBoxVGA

## How much RAM and hard disk space did you allocate to your VM? Why did you choose these amounts?
Base Memory is set to 4096 MB and 32 GB of Virtual Hard Disk. I selected these amounts because they were listed in the set-up instructions.
## What do you think would happen if you allocated too much RAM to your VM?
Increasing the RAM allocated will affect my PC's performance and may prevent me from performing background processes.
## What settings did you change and why?
I had to use sudo apt update. Sudo allows you to elevate privileges, apt applies installation, and then we forced an update. 

Then we installed the required packages through bzip2 build-essential gcc make perl dkms. This is required for future scripts we will input.

Then the instructions required us to enable 3D acceleration, which allows the VM to use more video memory, improving graphics quality. 

Then we enabled shared clipboard, which allows copied text to be input into the VM, which allows us to copy text instead of manually typing across systems.
## How did your VM perform before and after changing the settings?
Visually, it looked better, and now I can copy items into the VM, which will save a ton of time.
## What other settings do you think could be important for optimizing a VM’s performance?
I could increase the amount of memory allocated to the VM to improve processing. 

