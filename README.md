##Kautilya

###Kautilya-micro is a porting of Kautilya toolkit to Arduino-Micro platform.
Kautilya is developed by [nikhil_mitt](https://twitter.com/nikhil_mitt) and its original repository can be found [here](https://github.com/samratashok/Kautilya)

To generate Kautilya paylods compatible with Arduino Micro you have to carry out the following steps:

1. Download Kautilya-micro with git clone https://github.com/valerio-click/Kautilya-micro
2. Download Arduino-HID-Plus with git clone https://github.com/valerio-click/Arduino-HID-Plus 
3. run Kautilya with ruby Kautilya-micro/Kautilya.rb
4. select the
#####List of Supported Payloads
#####Windows
######Gather
- Gather Information
- Hashdump and Exfiltrate
- Keylog and Exfiltrate
- Sniffer
- WLAN keys dump
- Get Target Credentials
- Dump LSA Secrets
- Dump passwords in plain
- Copy SAM
- Dump Process Memory
- Dump Windows Vault Credentials

######Execute
- Download and Execute
- Connect to Hotspot and Execute code
- Code Execution using Powershell
- Code Execution using DNS TXT queries
- Download and Execute PowerShell Script
- Execute ShellCode

######Backdoor
- Sethc and Utilman backdoor
- Time based payload execution
- HTTP backdoor
- DNS TXT Backdoor
- Wireless Rogue AP
- Tracking Target Connectivity

######Escalate
- Remove Update
- Forceful Browsing

######Manage
- Add an admin user
- Change the default DNS server
- Edit the hosts file
- Add a user and Enable RDP
- Add a user and Enable Telnet
-  Add a user and Enable Powershell Remoting

######Misc
- Browse and Accept Java Signed Applet
- Speak on Target

#####Linux
- Download and Execute
- Reverse Shells using built in tools
- Code Execution
- DNS TXT Code Execution
- Perl reverse shell (MSF)

#####OSX
- Download and Execute
- DNS TXT Code Execution
- Perl Reverse Shell (MSF)
- Ruby Reverse Shell (MSF)


#####Payloads Compatibility
- The Windows payloads and modules are written mostly in powershell (in combination with native commands) and are tested on Windows 7 and Windows 8. 

- The Linux payloads are mostly shell scripts (those installed by default) in combination with commands. These are tested on Ubuntu 11.

- The OS X payloads are shell scripts (those installed by default) with usage of native commands. Tested on OS X Lion running on a VMWare

#####Usage
Run kautilya.rb and follow the menus. Kautilya asks for your inputs for various options. The generated payload is copied to the output directory of Kautilya.

The generated payload is an arduino sketch, ready to be used with Arduino IDE. Burn it to Human Interface Device of your choice and have fun!

#####Supported Human Interface Devices
In principal Kautilya should work with any HID capable of acting as a keyboard. Kautilya has been tested on Teensy++2.0 and Teensy 3.0 from pjrc.com. Updates about Kautilya can be found most of the times at my blog http://labofapenetrationtester.com/ and google group.

#####User Group
For any queries, discussions and feedback, post to official google group http://groups.google.com/group/kautilya-users or mail me at nikhil d0t uitrgpv at gmail.com 

#####Bugs and Feature requests
Raise an issue or post to the google group.

#####Dependencies
Kautilya needs colored, highline and artii (and win32console on Windows) gems. Use

bundle install

to install all the required gems.
#####Contributing
If you code in Ruby, you can contribute by helping in rebuilding UI of Kautilya. 
I am trying to make it an interactive shell based tool unlike the current menus based UI.

I am always looking for contributors to Kautilya. Please submit requests or drop me email.

#####Blog Posts
A five part blog post on my blog could be useful for those new to HID and Kautilya:

Part 1: http://labofapenetrationtester.blogspot.in/2012/04/teensy-usb-hid-for-penetration-testers.html

Part 2: http://labofapenetrationtester.blogspot.in/2012/04/teensy-usb-hid-for-penetration-testers_04.html

Part 3: http://labofapenetrationtester.blogspot.in/2012/04/teensy-usb-hid-for-penetration-testers_25.html

Part 4: http://labofapenetrationtester.blogspot.in/2012/05/teensy-usb-hid-for-penetration-testers.html

Part 5: http://labofapenetrationtester.blogspot.in/2012/09/usb-hid-for-pen-testers-part5.html

All posts related to Kautilya
http://www.labofapenetrationtester.com/search/label/Kautilya

#####Credits
Due Credits and Borrowed Code: I do not put credits of any borrowed code inside the payloads generated by Kautilya to save space. Credits and thanks are generally mentioned either in the description of payloads or accompanying blog post. If you think I missed any due credit, please let me know. I will add the credits with apologies.

