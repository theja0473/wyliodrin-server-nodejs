wyliodrin-server-nodejs
=======================

Wyliodrin Server JS

Install
=======

For beginners, we recommand downloading the SD Card Image from www.wyliodrin.com.

For advanced users, you may install Wyliodrin Server yourself. Please follow the 
instructions depending on your board.

Raspberry Pi
------------

Download the release branch and run the install script. Please read the script 
before running it.

    ./wyliodrin-server-raspberry-pi.sh

To enable Visual Programming without the other languages, please read and run the script

    ./wyliodrin-server-install-visual.sh


If you want to enable wireless, you need to modify your /etc/network/interfaces file
to use wyliodrin configuration

    auto lo                                                                                                                                     
                                                                                                                                                
    iface lo inet loopback                                                                                                                      
    iface eth0 inet dhcp                                                                                                                        
                                                                                                                                            
    allow-hotplug wlan0                                                                                                                         
    iface wlan0 inet manual                                                                                                                     
    #wpa-roam /etc/wpa_supplicant/wpa_supplicant.conf                                                                                           
                                                                                                                                            
    wpa-roam /usr/local/lib/wyliodrin/wireless/wireless.conf                                                                        
    iface default inet dhcp  

Licesne
-------
This is released under a dual license. 
For non comercial use, the GPL v2 is valid.
For comercial usesage, please contact Wyliodrin SRL
