#Setting Up the ADT Bundle
The ADT Bundle provides everything you need to start developing apps, including a version of the Eclipse IDE with built-in ADT (Android Developer Tools) to streamline your Android app development. If you haven't already, go download the [Android ADT Bundle](http://developer.android.com/sdk/index.html).

##Install the SDK and Eclipse IDE

1. Unpack the ZIP file (named `adt-bundle-<os_platform>.zip`) and save it to an appropriate location, such as a "Development" directory in your home directory.

2. Open the adt-bundle-`<os_platform>/eclipse/` directory and launch eclipse.

The IDE is already loaded with the Android Developer Tools plugin and the SDK is ready to go.

#Sample Projects List

* [Location Demo](#location-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/android-LocationDemo).
* [Tab View Demo](#tab-view-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/Android-TabView-Demo).
* [Seek Bar Demo](#seek-bar-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/Android-seek-bar-demo).
* [Google Map Demo](#google-map-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/Google-Map-Demo-Project).
* [Video Player Demo](#video-player-demo)		Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidVideoPlayerDemo).
* [Timer Task Demo](#timer-task-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/TimerTaskDemo).
* [View Pager Demo](#view-pager-demo)			Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/Android-View-Pager-Demo).
* [Facebook Login Demo](#facebook-login-demo)		Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidFacebookLoginDemo).
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
* [Beacon Demo](#beacon-demo)				Source Code : [Github link](https://github.com/ranvijaySingh-Webonise/AndroidBeaconDemo).

###Location Demo
* This application shows how to program you application to show the current location of the mobile.
* This generally uses the longitude and the latitude of accesses from the GPS or from the Network. 
* You need to add few permissions in the manifest file and write a class to use the functions of LocationListener class. 

* There are few steps to do this : 
	* **Step 1 :** Give the permission in the android manifest file. 
	* **Step 2 :** Create the main class to handle the operation for button , when clicked. 
	* **Step 3 :** Create a class extending from the Service class and implement LocationListener. 

###Tab View Demo
* This is a sample application to create a TabView demo. 
* The application contain two tabs which handles two different fragment in the application.
* The main points that you have to remember is the naming the ids.
i.e. In the layout the TabHost tag has to be `android.support.v4.app.FragmentTabHost` and its id will be `android:id="@android:id/tabhost` instead of ` android:id="@+id/tabhost`.
similarly the TabWidget tag id will also be like this ` android:id="@android:id/tabs `

* The steps to follow is as follows :
	* **Step 1 :** Creating the main layout `activity_main.xml`.
	* **Step 2 :** Create two other fragment layout . ie `tab1.xml` and `tab2.xml`. …`tab1.xml`
	* **Step 3 :** Create the two classes extending the fragment . First is `Tab1Fragment.java`
	* **Step 4 :** Creating the main activity `MainActivity.java`. In this file you have to be careful to give the id correctly . ie. `mTabHost = (FragmentTabHost) findViewById(android.R.id.tabhost); `

###Seek Bar Demo
* This is a demo application that demonstrate the use of seek bar to change the image in a imageview.
* The layout of the page contains the image view at the top with a seek bar at the bottom . 
* The main function is to change the image on moving the seekbar.
	* **Step 1 :** The main layout file contain a framelayout that will manage the fragments dynamically. the file is `activity_main.xml`.
	* **Step 2 :** The second layout is containing the image view with a seek bar. `image_fragment.xml`
	* **Step 3 :** Create a class extending fragment that will contain the basic functions `ImageFragment.java`.
	* **Step 4 :** This is main activity that add the fragment in the frame layout `MainActivity.java`.

###Google Map Demo
* This is a tutorial for using the google map in you application .
* There are few very simple steps to create the application. 
	* **Step 1 :** Creating your SHA-1 key . 
	* **Step 2 :** Getting access to the google map api. 
	* **Step 3 :** Adding premissions to the android mainfest file . 
	* **Step 4 :** Creating the layout for the map. 
	* **Step 5 :** Creating the java class to handle the map view.

###Video Player Demo
* This application to show the use of a media file from the RAW folder in the application directory.
* There are very simple steps to add and use the video file in your application.
* The steps to follow are as follows : 
	* **Step 1:** Create a new Folder named `raw` in your `res` directory and add the video files.
	* **Step 2:** Create a layout using the VideoView object.
	* **Step 3:** Create the java file for the layout.

###Timer Task Demo
* This application demonstrate the use of the Timer and the TimerTask to show a timer that starts from 0 and count till the user input.
	* **Step 1:** The layout is very simple containing only one text view `acitivity_main.xml`.
	* **Step 2:** This is the main java file to handle the runnable objects nadn the counters : `MainActivity.java`.

* For the explanation ... scheduleAtFixedRate : has three parameters 
		new TimerTask() - task 
		100 - after how many milliseconds the run function should start. 
		1000 - what is the delay in milliseconds

###View Pager Demo
* This is a demonstration for creating a page view in an application.
* The steps to follow are very simple and easy to understand .
	* **Step 1 :** In the main layout “activity_main.xml ”
	* **Step 2 :** Create the next views .ie. first page , second page and third page.
		In my case 
		First page has a text view ,
		Second page has image view and 
		Third page has a image view.

###Facebook Login Demo
* This application a demo to show how to use the facebook login as to login in to your app . 
* There are a particular set of steps that you need to follow . 
* These steps are well defined by the [facebook developers](http://developers.facebook.com/docs/android/getting-started/facebook-sdk-for-android/).

* I will assume you have the facebook sdk and you have successfully installed it . 
	* **Step 1:** Generate you Hash key . 
	* **Step 2:** Create new application . 
	* **Step 3:** Register you app with the facebook using hash key and get the application ID. 
	* **Step 4:** Fill the details of the `Android Native Application`. 
	* **Step 5:** Create a string with a application id in `string.xml`. 
	* **Step 6:** Add the permission to your manifest file . 
	* **Step 7:** Create the main java file `MainActivity`.

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

###Beacon Demo
* This application shows how to use the android phone as a monitor for the beacon devices.
* For this we are using the Radius Networks API.
* This application monitors the distance between the beacon and the monitoring device(your application).
* First you have to get the APIs that will be needed in this application.
You can download it from this link : 
[radiusNetwork](http://developer.radiusnetworks.com/ibeacon/android/download.html).

After downloading 
import the project as a library in your application.

*These are the steps that you need to follow
	* **Step 1:** Give the permission in the manifest file and declare few services.
	* **Step 2:** Create a simple layout.
	* **Step 3:** Write the main class.

