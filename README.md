## Fork of rickfarmer's android vm

This is a vagrant box that preloads JDK7, Android Studio, the Android SDK/Build Tools, the Android NDK, GNU C/C++  tool-chain, apt, and vim. It runs on Ubuntu 12.04 (64 bit).

###Instructions
==============

####Install Components
For your VM environment, you will need:   
[Vagrant](https://www.vagrantup.com/downloads.html)   
[Oracle VirtualBox](https://www.virtualbox.org/wiki/Downloads)

Make sure you update your path variable.


####Clone the repository

You'll need [git](http://git-scm.com/) if you don't already have it.   
Open a terminal.       
Create a directory where you will do your development.      
From that directory, run `git clone https://github.com/masterjefferson/android-vm`      
`cd` into the `android-vm` directory and enter `git submodule init`      
Then, enter `git submodule update`      
You're now ready to bring up the VM!      

####Vagrant up!

While still in the `android-vm` directory, enter `vagrant up`.
The provisioning can take a *long* time, over 20 minutes is normal. Be *patient*.   
Once provisioning is completed, enter `vagrant reload`. You should be greeted with a login screen.
Username: vagrant Password: vagrant   

####Further configuration   
If the VM is running, enter `vagrant halt`    
Open up VirtualBox and select your machine. Click settings.   
I reccommend setting the video ram to max, cpu to max, and systam ram to 1/4 of your total ram.

####Where are my tools?
Android development tools were installed to `/usr/local/android`


####Issues
Git installation is missing (Can still be installed from inside VM). Fix coming.   
Missing Android API 21 tools/images (API 22 is installed though). Fix coming.



