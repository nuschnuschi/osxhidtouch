osxhidtouch
===========

User-space HID multitouch touchscreen driver for Mac OS X. 
Fork for Thinkpad T440s's Elan Microelectronics TouchScreen

How to install:

1. Build it then put it to /usr/bin/

2. In Terminal,
sudo chown root:wheel /usr/bin/HidTouch
sudo chmod 755 /usr/bin/HidTouch

3. Create a .plist and put it to /Library/LaunchDaemons/

ex.) org.yourname.hidtouch.Daemon.plist

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList$ <plist version="1.0">
<dict>
        <key>Label</key>
        <string>org.yourname.hidtouch.Daemon</string>
        <key>RunAtLoad</key>
        <true/>
        <key>KeepAlive</key>
        <false/>
        <key>Program</key>
        <string>/usr/bin/Hidtouch</string>
</dict>
</plist>
