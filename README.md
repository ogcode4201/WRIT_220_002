#**Crouton**  
 
##Background - The Chromebook
In 2011 Google released their first iteration of the Google Chromebook. There have been an array of models ranging in hardware specifications from different vendors since then. Chromebooks signature is it’s lightweight, thin-client Operating System(OS). Chrome OS is geared towards the general user. More advanced users can find the Chrome-OS restricted and limiting as much of the functionality of Chrome-OS depends on a persistent internet connection. Despite these shortcomings, Chromebooks have moderate amount of success in the consumer electronic market due to their well thought out design, reasonable hardware performance, slim profile, excellent battery life, and generally low cost. 

##The Purpose of Crouton 
  Crouton stands for **C**h**R**omium **O**s **U**niversal chroo**T** envir**ON**ment, and is a bundle of scripts utilized to load a distribution of Ubuntu Linux that runs alongside, and shares system resources with Chrome OS. crouton transforms the Chromebook from a simple net book to functional laptop with the extended capabilities offered by a robust Linux distribution.

##How it works
crouton works by installing a Linux distribution and desktop environment on a new mounting point of the root directory known as a chroot. This guest OS allows for additional software to be installed and run which was not available for the original ChromeOS. Because both ChromeOS and the installed Linux distribution are Unix based systems, they are able to share many of the lower level software that interacts directly with the hardware. It is because of this that both OSs are able to maintain a stable running environment without significant load increase on the memory and processor.



####Chroot
A chroot, or **CH**ange **ROOT** is when the root directory of the system is changed to a different mounting point in the file structure.
   Chroots are typically used in security purposes to lock out digital intruders from important directories by placing them in their own set of directories that are secured from the main system. This application is known as a _Chroot jail_. In the case of Crouton however, the chroot is created for the the Linux distribution to use, keeping a level of separation between the two operating systems file systems but allowing for the guest OS to share resources with the ChromeOS.
    
####The Linux Distribution  

Ubuntu Linux is one of the default distributions installed using Crouton. Other distributions can be installed such as Debian and Kali. A full list of supported distributions can be found via the command line. 
Ubuntu is a user friendly Linux distribution. It is also easy to install and configure, making it a excellent candidate for a users first chroot installation. Kali is a distribution of Linux created with information security applications in mind and comes with a large array of tools pre-installed with this purpose. It is a more technical version of Linux recommended for advanced users.

   
####The Desktop Environment
Several options exist for runtime options with Crouton. Due to the low graphic processing capabilities and shared ram with the native ChromeOS, a lightweight Desktop environment such as XFCE is recommended. Systems with more ram and graphical processing capability will run  environments such as Unity but results may vary.

##Is Crouton the same thing as Dual-Booting?
 
Crouton is frequently confused as a Dual-boot solution, this however is inaccurate in some    important ways:



  
* **no rebooting to switch OSs**    
     _with crouton you can seamlessly switch between two(or more) OSs with a keyboard shortcut, allowing for easy multitasking between OSs that isn’t possible on a dual-boot platform _

* **no hard drive partitioning**  
 _Dual boot systems partition the hard drive into sections that are off limits to the other OS, crouton allows for multiple OSs to run on a single hard drive without this division, this allows for shared directories and files and system resources._     
     
* **OS Synergy**   
 _By taking advantage of the strengths of both OSs, Crouton offers the intermediate and advanced user a convenient synergy-centric solution._

##**Important Considerations for the User**  
###Software Availability  
what software available to the user will depend heavily on which distribution of Linux has been installed. Some versions are supported by the Open Source community better than others, take this into consideration when choosing the right Linux for you. 
 
###Software Compatibility  
Unforseen software compatibility issues may occur. Individuals are encouraged to find and share their own solutions to such issues. Forums usually exist for individual open source projects and for individual Linux distributions. These communities can be a wealth of knowledge for errors and fixes.

###Data Integry  
system stability may vary depending on your hardware and software configuration,
use of Crouton could result in loss of data. **All users are encouraged to back up their data frequenty.** any loss of data is the sole responsibility of the user.

###Security concerns  
Crouton has not had extensive penetration testing therefore use of Crouton on a Chromebook could potentially expose security vunerabilities. **Crouton should not be used on any system containing sensitive information of any kind or in any application where security is a concern!** System security is the sole responsibility of the user.

###Hardware Warranty 
 **Crouton may void your warranty, refer to the terms and conditions of the manufacturer and technical service providers before using Crouton**

###Hardware Performance  
 Crouton in no way improves the performance of the Chromebook's hardware, rather it provides alternate way of interacting and utilization of that hardware that is not possible with the default OS alone, lower end machines may see impact in performance. Your Chromebook's hardware specifications should be considered when choosing how to configure your chroot and choosing which desktop environment to use.  




##Contribution information
Contributors are welcome but must first sign a [Contributor License Agreement](https://cla.developers.google.com/clas/new?kind=KIND_INDIVIDUAL&domain=DOMAIN_GOOGLE) additional information  [here](https://github.com/dnschneid/crouton#i-want-to-be-a-contributor)

##License info

Please review [this BSD license](https://github.com/dnschneid/crouton/blob/master/LICENSE) before using or modifying the source code.


##Additional information and Download  
Visit the [Official Crouton Github](https://github.com/dnschneid/crouton) for the download link.  
Additional information can be found at the [Crouton wiki.] (https://github.com/dnschneid/crouton/wiki)






 


    










