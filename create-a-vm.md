# Create a VM lab

## Your first VM
### What OS is your VM running? 
My VM is running Ubuntu
### What challenges did you face while creating your VM? What troubleshooting steps did you take to resolve those challenges and what did you research?
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

### How much RAM and hard disk space did you allocate to your VM? Why did you choose these amounts?
Base Memory is set to 4096 MB and 32 GB of Virtual Hard Disk. I selected these amounts because they were listed in the set-up instructions.
### What do you think would happen if you allocated too much RAM to your VM?
Increasing the RAM allocated will affect my PC's performance and may prevent me from performing background processes.
### What settings did you change and why?
I had to use sudo apt update. Sudo allows you to elevate privileges, apt applies installation, and then we forced an update. 

Then we installed the required packages through bzip2 build-essential gcc make perl dkms. This is required for future scripts we will input.

Then the instructions required us to enable 3D acceleration, which allows the VM to use more video memory, improving graphics quality. 

Then we enabled shared clipboard, which allows copied text to be input into the VM, which allows us to copy text instead of manually typing across systems.
### How did your VM perform before and after changing the settings?
Visually, it looked better, and now I can copy items into the VM, which will save a ton of time.
### What other settings do you think could be important for optimizing a VM’s performance?
I could increase the amount of memory allocated to the VM to improve processing. 


## Your second VM
### What OS is your VM running? 
My VM is running Windows 10
### What challenges did you face while creating your VM? What troubleshooting steps did you take to resolve those challenges and what did you research?
I initially could not get the OS to boot without a product key. After watching the YouTube video titled <a href="https://www.youtube.com/watch?v=CMGa6DsGIpc&t=23s">How to install Windows 10 in VirtualBox 2024</a> which explained that I had to  select "Skip Unattended Setup" when creating my VM in VirtualBox.        

**Steps to correct in the future:**
When creating your virtual machine:
1. Select the ISO image titles Windows.iso
2. Under the Windows version, select Skip Unattended Installation.


### How much RAM and hard disk space did you allocate to your VM? Why did you choose these amounts?
Base Memory is set to 11956 MB, an increase from the initial 4096 MB. This was increased because immediately, my Curser and Applications were incredibly slow, and I knew that my PC would handle the increased Ram allocation.  
I increased my Hard Disk space to 50 GB because the OS itself was 11 GB, and I wanted to give my VM room for other programs.

### What do you think would happen if you allocated too much RAM to your VM?
Like I mentioned in the first VM lab, too much allocated RAM will affect my PC's performance and may prevent me from performing background processes.

### What settings did you change and why?
I tried to personalize my desktop, but unfortunately, this would require a product key. 

Then I enabled shared clipboard again, which allows copied text to be input into the VM, which allows us to copy text instead of manually typing across systems.

### How did your VM perform before and after changing the settings?
My performance was positively impacted by increasing the allocated RAM, but the other settings were purely for convenience., 
### What other settings do you think could be important for optimizing a VM’s performance?
When I opened Task Manager to monitor CPU and Memory usage to ensure that there was no peaking, there was a brief period when the CPU was maxed out when I was setting up Edge, but it settled at 2-10%. 
Because this VM does not have a set intended use yet and is clean of any interfering programs, I do not need to adjust the allocated CPU, RAM, or Hard Drive capacity. The system still lags a little bit, which I will need to look into more. A few Reddit threads suggested disabling the firewall, which I may try in the future, but at this time, it works for where we are within this course. 



