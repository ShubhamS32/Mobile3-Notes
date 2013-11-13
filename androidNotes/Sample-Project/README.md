#Setting Up the ADT Bundle
The ADT Bundle provides everything you need to start developing apps, including a version of the Eclipse IDE with built-in ADT (Android Developer Tools) to streamline your Android app development. If you haven't already, go download the [Android ADT Bundle](http://developer.android.com/sdk/index.html).

##Install the SDK and Eclipse IDE

1. Unpack the ZIP file (named `adt-bundle-<os_platform>.zip`) and save it to an appropriate location, such as a "Development" directory in your home directory.

2. Open the adt-bundle-`<os_platform>/eclipse/` directory and launch eclipse.

The IDE is already loaded with the Android Developer Tools plugin and the SDK is ready to go.

#Sample Projects List

* [Service Demo](#service-demo)				Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidServiceDemo).
* [Dynamic Fragment Demo](#dynamic-fragment-demo)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidDynamicFragmentDemo).
* [Internet Connection Demo](#internet-connection-demo)	Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/CheckConnectionDemo).
* [Twitter Login Demo](#twitter-login-demo)		Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/Android-Twitter-Login-Demo).
* [Expandable List View Demo](#expandable-list-view-demo) Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/Android-Expandable-List-View-Demo).
* [Grid View Demo](#grid-view-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/Android-GridViewDemo).
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

###Service Demo
* This application shows how to run a service in the background of a application. 
* There are 4 basic steps to do this : 
	* **Step 1:** Giving the entry in the `Mainfest file`. 
	* **Step 2:** Creating the xml layout ` acitivty_main.xml `
	* **Step 3:** Creating myService Class . `MyService.java`
	* **Step 4:** Creating the mainActivity class to handle the service request ` MainActivity.java `

###Dynamic Fragment Demo
* This application sample will show you how to handle the fragments in a application based on the user click. 
* There are very specific steps to do this . 
	* **Step 1:** Create your layout for the fragments . 
	* **Step 2:** Create your fragments classes. 
	* **Step 3:** Create your main Activity `MainActivity.java` 

Now to understand the concept of fragment you need to know about few function and methods that fragments need to execute . 

* FragmentManager : (Abstract Class) - interface to interact with the fragment with Activity. 
* FragmentTransaction : (Abstract Class) - API for performing a set of Fragment operations. 
	* Transaction should be performed every time you shift from one fragment to another---- 
	- FUNCTIONS- 
		-add() : adds a complete new Fragment to the UI. 
		-remove() : removes the fragment from the activity. 
		-replace() : replace the existing fragment that was added to layout. 
		-commit() : make you fragment visible to the UI. 
	* there cannot be more than one commit on a fragment --- 
	* if you need to commit the present fragment , replace or remove the previous fragment---

###Internet Connection Demo
* This is a demo project to demonstrate how to check for internet connection and any other network connection . 
* The steps are very easy .
	* **Step 1:** Give user-permission in the android manifest file . 
	* **Step 2:** Create a separate class to check for the internet connection. 
	* **Step 3:** Call the class function in the main acitivity.

###Twitter Login Demo
* This application shows the use of Twitter in your application.
* The very first thing you need is the Twitter account. 
* Once you have the account you need to generate the Api keys. ie.`Customer key` and `Consumer key`.

* There are very simple steps to do this :
	* **Step 1:** Go to [twitter dev](https://dev.twitter.com/apps/new) and register new application.
	* **Step 2:** Give some dummy url in the callback url field to make the app as browser app.
	* **Step 3:** Under the settings tab upload icon and change the access type to Read and Write.
	* **Step 4:** Copy Consumer Key & Consumer Secret key. 
	* **Step 5:** Download & extract twitter4j library from twitter4j-android-2.2.6.zip (slimmed version for Android platform). 
	* **Step 6:** In your mainifest file give the permissions and add the new intent filter.
	* **Step 7:** Create the new Class to check for the connection and network `ConnectionDetector.java`.
	* **Step 8 :** In the main Activity give the access to the twitter login `MainActivity.java`

###Expandable List View Demo
* This application shows how to use the expandable ListView in an application .
* The most the concept is same as the listView .
* In the ListView we use to use the adapter `BaseAdapter` to add elements to the list ,whereas in Expandable listView we use `ExpandableBaseAdapter` to add elements to the list . 
* These steps will guide you to get to the bottom on the working of the list view. 
	* **Step 1:** Create the main activity layout to hold the ExpandableListView element.
	* **Step 2:** Create the layout to hold the parent list elements .
	* **Step 3:** Create the layout to hold the child list element .
	* **Step 4:** Create the adapter which will populate the list view.
	* **Step 5:** Create the main activity class that can create the list on header data and list of child data. Its better to use the list of strings for the header data and hashmap to hold the child data.

###Grid View Demo
* This application will show how to add grid view in an application .
* All you need is additional adapter that populates the grid elements .
* Steps to follow are as follows : 
	* **Step 1 :** Create the Layout for the main Activity containing a gridView.
	* **Step 2 :** Create the adapter class “ImageAdapter.java”.
	* **Step 3 :** Create the main Activity class . “MainActivity.java”

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
