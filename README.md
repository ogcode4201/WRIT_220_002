#**Crouton**  
 
##Background - The Chromebook
In 2011 Google released their first iteration of the Google Chromebook and since then, there have been an array of models ranging in hardware specifications from different vendors. Chromebooks signature is it’s lightweight, thin-client Operating System(OS). Chrome OS is geared towards the general user. More advanced users can find the Chrome-OS restricted and limiting as much of the functionality of Chrome-OS depends on a persistent internet connection. Despite these shortcomings, Chromebooks have moderate amount of success in the consumer electronic market due to their well thought out design, reasonable hardware performance, slim profile, excellent battery life, and generally low cost. 

##The Purpose of Crouton 
  David Schneider, A senior hardware engineer at Google, wanted to take the strengths of the Chromebook and extend the functionality of the chromebook to compete with Mac or Windows systems. With these goals in mind he developed crouton. crouton stands for **C**h**R**omium **O**s **U**niversal chroo**T** envir**ON**ment, and is a bundle of scripts utilized to load a distribution of Ubuntu Linux that can run alongside Chrome OS. crouton transforms the Chromebook from a simple net book to functional laptop with the extended capabilities offered by a robust Linux distribution.

##How it works?  
crouton works by installing a Linux distribution and desktop environment on a new mounting point of the root directory known as a chroot.



####Chroot- the change root command
   Chroots are typically used in security purposes to lock out intruders from important directories by placing them in their own set of directories locked out from the main system known as a _Chroot jail_. In this case however the chroot is created for the the Linux distribution to use, keeping a level of separation between the two operating systems file systems but allowing for the guest OS to share resources with the ChromeOS.
    
####The Linux Distribution  
Ubuntu Linux is the default distribution installed using Crouton. Other distributions can be installed, but they are not supported and results may vary.  
Ubuntu is a user friendly Linux distribution. It is also easy to install and configure, making it a excellent candidate for scripted installation with Crouton.

   
####The Desktop Environment
Several options exist for runtime options with crouton. Due to the low graphic processing capabilities and shared ram with the native ChromeOS, a lightweight Desktop environment such as XFCE is recommended. Systems with more ram and graphical processing capability will run  environments such as Unity but results may vary.

##Is Crouton the same thing as Dual-Booting?
The short answer is no, however...  
Crouton is frequently confused as a Dual-boot solution, this however is inaccurate in some    important ways:
  
+no rebooting to switch OSs - with crouton you can seamlessly switch between two(or more) OSs with a keyboard shortcut, allowing for easy multitasking between OSs that isn’t possible on a dual-boot platform  
+no hard drive partitioning- dual boot systems partition the harddrive into sections that are off limits to the other OS, crouton allows for two OSs to run on a single hard drive without this division, this allows for shared directories and files. This can be complicated to set up in a dual-booting configuration.
     OS Synergy- the hardcore do-it-yourself computer user may think it more advantages to simply wipe ChromeOS completely and run another OS entirely, and with the proper technical skills and a specific purpose for their machine this may be the case. however for the more intermediate users ,crouton offers the advantage of OS-Synergy
downside to ubuntu
Ubuntu is an open source OS and so is most of the software designed to run on the platform, this results in a large variety of tools and programs which vary wildly in quality. Ubuntu is the jack of all trade but master of none among Linux distributions other Linux distributions may be specialized for a certain task (such as Chrome OS) but they lack flexibility that a student or computer hobbyist may desire
Chrome OS, a commercial distribution of Linux created by Google is    specialized with a focus on web and cloud integration, ChromeOS is a master of its specific purpose but lacks support to expand into other areas such as software development or audio/video editing
together these two OS compliment each other to take full advantage of the hardware capabilities
    
    

D. the down side - crouton is an open source project without the full funding or support of Google, and as such it has been lightly tested with almost no penetration tests. Because of this serious security vulnerabilities can be opened by using crouton and it is not recommended on systems that handle personal or work information that is considered sensitive.


E what crouton isn’t
    crouton in no way improves the performance of the chromebook's hardware, rather it provides alternate way of interacting and utilization of that hardware that is not possible with the default OS, lower end machine can see a notable degradation of performance and your chromebook's hardware specification should be considered when choosing how to configure your chroot, and choosing which desktop environment to choose  








