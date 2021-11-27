# TrollPPlwithJailbrokenDevices
This is a tutorial how to connect to jailbroken device that are in the same network like you or that are connceted to your device trough cable

# SSH to devices in your Network /  Get targets ip address
In case you don´t know the tragets iP address, but your are sure its in the same network, open Terminal and type:
arp -a
It will show you a list of all devices in the network (Device Name + iP address) (for example: myipad-name.WIFI.BOX.OR.ROUTER.NAME (xxx.xxx.xxx.xx) at a:x:xx:yx:xx:xx on en0 ifscope [ethernet] 
x = a number and y = letter i just don´t want to put mine in here. 
You need to copy ths number that are in brackets (xxx.xxx.xxx.xx) but don´t copy the brackets

## SSH Part
open terminal and type: ssh root@xxx.xxx.xx 
xxx.xxx.xxx.xx is the ip address
After you typed it you will maybe need to type yes or no, just type yes and hit enter
Now type in the targets root password. Thats the problem now, the default password is "alpine" so you can hope that the user of the target device never changed it and type alpine. When alpine will not work, you need to bruteforce the passcode :/

When you are in type any command you want. I will add later how to send UIAlerts after logging in
