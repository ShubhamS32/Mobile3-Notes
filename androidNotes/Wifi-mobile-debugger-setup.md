We know how to use the mobile for debugging using the  usb connection. </br>
We even know how to run an apk file by transferring the apk through airdroid .</br>

NOW lets know to use a new method of debugging without the use of the cables or airdroid , but you need to use few of the terminal commands to do the setup.

####Step 1:#### Connect your mobile using the usb cable. (make sure you can see the device in the eclipse in the device tab).

*Step 2:* Open the terminal and go to directory “android-sdk-mac_x86/platforms-tools/” or type  this command 
		cd android-sdk-mac_x86/platform-tools/

*Step 3:* Give this command 
		./adb devices
	this command shows all the devices that are compatible with the eclipse .(your device will be one of them.)

*Step 4:* Kill all other devices (emulators) that are shown except your own mobile.

*Step 5:* In the terminal give the following commands 
		./adb tcpip 5555
	this command assigns a port to the device .

*Step 6:* Then give this command 
		./adb connect 192.168.10.138
	if you get this message “connected to 192.168.10.138:5555”
	WALLAAAAA…. you are good to go .
if not then 
 do this  
	give the command 
		./adb usb
	this command reset the usb ports and the devices then repeat the above process from step 3 onwards.

