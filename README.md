LEDVIEWER
=========

ON/OFF & PULSE LED - PYTHON SCRIPT FOR RASPBERRY PI (step by step for dummies)
phone/tablet led remote/wireless control via temviewer  and a windows pc

NEEDED
- 1° led
- 1° 270 or 300 ohm resistor
- connect the resistor to the cathode of the led
- connect the resistor at pin 12(gpio 18) GPIO 
- connect the anode of the led at pin ground(gpio 6) GPIO

RASPBERRY PI
- open lx terminal 
   - type: sudo idle 3
- file-new window: type the "ledviewer" script
- save script on raspberry directory
- right click on script-properties-permissions- then select: make the file executable
    - in lx terminal type: ifconfig
- note your ip adress (eth0 inet addr)

WINDOWS 
- download and install xming(free xserver)
- download and install putty (free ssh client)
- download and install temviewer (free remote control)
- open and configure xming: multiple windows - start no client - label "clipboard"- save configuration-end
- open and configure putty: type ip adress - in connection type, in left bar open ssh and select x11-label enable x11- forwarding
                                                                                                                     - mit-magic-cookie
- save configuration with name and click "open"
- type pi login and password
- at raspberry prompt type: startlxde
- you're in!
RASPBERRY PI AND WINDOWS
- now go to raspy menu-applications-accessories- open "root terminal" (be careful)
                                               - type: cd /yourscript directory/ (ex: /home/pi/desktop)
                                               - type: python LEDABI.py (or the new name you gave to the script)
- the scipt start in a new (tk)window (there are three buttons: on - off - puls(a)
- open teamviewer on windows

PHONE/TABLET

- download and install teamviewer (for free)
- open teamviewer 
- type id and password
- enjoy!
                                                                                       
                                                                                  