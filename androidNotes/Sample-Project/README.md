#Setting Up the ADT Bundle
The ADT Bundle provides everything you need to start developing apps, including a version of the Eclipse IDE with built-in ADT (Android Developer Tools) to streamline your Android app development. If you haven't already, go download the [Android ADT Bundle](http://developer.android.com/sdk/index.html).

##Install the SDK and Eclipse IDE

1. Unpack the ZIP file (named `adt-bundle-<os_platform>.zip`) and save it to an appropriate location, such as a "Development" directory in your home directory.

2. Open the adt-bundle-`<os_platform>/eclipse/` directory and launch eclipse.

The IDE is already loaded with the Android Developer Tools plugin and the SDK is ready to go.

#Sample Projects List

* [Animation Demo](#animation-demo)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidAnimationDemo).
* [NfcTag Reader Demo](#nfctag-reader-demo)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidNfcReaderDemo).
* [NfcTag WebService Demo](#nfctag-webservice-demo)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidNfcWebServiceDemo).
* [NfcTag Writter Demo](#nfctag-writter-demo)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidNfcTagWritterDemo).

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
