osxhidtouch
===========

User-space HID multitouch touchscreen driver for Mac OS X.   
Fork for Thinkpad T440s's Elan Microelectronics TouchScreen.

How to install:

1. Build it then put it to /usr/bin/

2. In Terminal,  
sudo chown root:wheel /usr/bin/HidTouch  
sudo chmod 755 /usr/bin/HidTouch  

3. Copy 'org.osxhidtouch.hidtouch.Daemon.plist' to /Library/LaunchDaemons/

4. Reboot
