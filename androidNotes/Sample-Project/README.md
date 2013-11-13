#Setting Up the ADT Bundle
The ADT Bundle provides everything you need to start developing apps, including a version of the Eclipse IDE with built-in ADT (Android Developer Tools) to streamline your Android app development. If you haven't already, go download the [Android ADT Bundle](http://developer.android.com/sdk/index.html).

##Install the SDK and Eclipse IDE

1. Unpack the ZIP file (named `adt-bundle-<os_platform>.zip`) and save it to an appropriate location, such as a "Development" directory in your home directory.

2. Open the adt-bundle-`<os_platform>/eclipse/` directory and launch eclipse.

The IDE is already loaded with the Android Developer Tools plugin and the SDK is ready to go.

#Sample Projects List

* [Google Direction](#google-direction)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidGoogleDirection).
* [Google Direction](#google-direction)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidGoogleDirection).
* [Google Direction](#google-direction)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidGoogleDirection).
* [Bluetooth Demo](#bluetooth-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/androidBluetoothDemo).
* [CheckBox Demo](#checkbox-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidCheckBoxDemo).
* [GridView Image Selector](#gridview-image-selector)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/Android-GridView-ImageSelector).
* [Profile Changer Demo](#profile-changer-demo)		Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidProfileChangeDemo).
* [Mobile Viberation Demo](#mobile-viberation-demo)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidViberateDemo).
* [Google Direction](#google-direction)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidGoogleDirection).
* [Web Service Demo](#web-service-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidWebserviceDemo).
* [Animation Demo](#animation-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidAnimationDemo).
* [NfcTag Reader Demo](#nfctag-reader-demo)		Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidNfcReaderDemo).
* [NfcTag WebService Demo](#nfctag-webservice-demo)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidNfcWebServiceDemo).
* [NfcTag Writter Demo](#nfctag-writter-demo)		Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidNfcTagWritterDemo).

###Bluetooth Demo
* This application shows you how to use bluetooth of the device.
* The function is there to enable and disable the bluetooth and to make the device discoverable.
* The steps involved in this process is as follows :
	* **Step 1:** Add permission to the uses in android mainfest file.
	* **Step 2:** Create the layout of buttons to start and stop the bluetooth.
	* **Step 3:** Create the class to use enable the bluetooth functions.

###CheckBox Demo
* This application shows working of a checkbox in android. 
* The checkBox is very much similar to other objects in the android UI Design.
* These are the steps to show how a checkbox works.
	* **Step 1:** Create the layout.
	* **Step 2:** Create the class to handle the check events.

###GridView Image Selector
* This application shows how to create a Grid view of images.
* Every image has a check box on it which is allows you to select more then one image at a time.

###Profile Changer Demo
* This application shows how to change the phone profile from normal to silent and from silent to normal in an application. 
	* **Step 1:** Create the layout with two buttons. 
	* **Step 2:** Create the class to handle the onclick functions to change the profile . 

###Mobile Viberation Demo
* This application shows how to use the mobile vibrate service in your application.
* To use this service you need to access the system settings for that you need to add few permission to the manifest file .

		<uses-permission android:name="android.permission.VIBRATE" />

and to receive the service you need to use the receiver as a class and you need to show the receiver class to the mainifest file as well .

		<receiver android:name="MyBroadCastReceiver" >
        	</receiver>

* There are are very few steps that you need to follow to create this application.
	* **Step 1:** Create the layout with one edit text and a button .
	* **Step 2:** Give the permission in the mainfest file .
	* **Step 3:** Create the class to handle the call for the alert message operation .

###Google Direction
* This is a demo project to use the google map to show the direction in google map . 
* There are few sets of requirements and topics that you need to understand before you begin to play with the google map .

**Ployline :** This term is not so clear . 
	Let me rephrase it , line joining two points. 
	* In google map when you have to show the direction between two points then you have to use multiple points and then join all the points to show a complete curved path .

* To obtain these points you have to use the webservice to get the list of point or list of LatLong.

###Web Service Demo
* This project demonstrate how to use the webservice in your project.
* Accessing the web service is very simple thing.All you need to do is to use few objects to initialize and send request like :
	* HttpGet 
	* HttpRequest
	* HttpResponse.

###Animation Demo
* This application show how to use the xml file to create animation in an application . 
* Similar to the OnClickListener we are using AnimationListener to set animation on any object .
* There are very few steps to use animation in your application. 
	* **Step 1:** Create the xml file with the animation.
	* **Step 2:** Create the layout .
	* **Step 3:** Create the class to use the animation object .

###NfcTag Reader Demo
* This application shows how to read a nfc tag in your application .
* The data written on the NFC is displayed as a toast(popup).

###NfcTag WebService Demo
* Application show how to hit an API once you tap on the tag.
* The API hit returns a response which is displayed on the application.

###NfcTag Writter Demo

* This application shows how to write in a nfc tag.
* Tap on a tag to launch your application  even when there are other application present on on the mobile.
