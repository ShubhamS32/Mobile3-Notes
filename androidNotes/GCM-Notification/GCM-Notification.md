# Google Cloud Messaging (GCM) Notification

Google Cloud Messaging (GCM) is a service that allows you to send data from your server to your users' Android-powered device.
This could be a lightweight message telling your app there is new data to be fetched from the server and it could be a message containing up to 4kb of payload data

## How GCM Works




















1. First android device sends sender id,application id to GCM server for registration.
2. Upon successfull registration GCM server issues registration id to android device.
3. After receiving id, device will send registration id to our server.
4. Our server will store registration id in the database for later usage

A. Whenever push notification is needed,our server sends a message to GCM server along with device registration id (which is stored earlier in the database)
B. GCM server will delevers that message to respected mobile device using device registration id

# Regitering to Google Cloud messaging
 Getting your Sender ID
                                    

STEP 1.  Register Here .
STEP 2.  Click Create project. Your browser URL will change to something like:
" https://code.google.com/apis/console/#project:4815162342 "
Take note of the value after#project: (4815162342 in this example). This is your project ID, and it will be used later on as the GCM sender ID. This Id will be used by the Android Device while Registering for Push Notification.
STEP 3. Choose Service tab from the left side menu on the web page. and turn on “ Google Cloud Messaging for Android “
STEP 4. Go to API Access tab from the left menu of web page.
press Create new Server key and note down the generated key

## Before Create an application

1. Update ADT plugin 20 .
2. update SDK > install Extras > Google Cloud Messaging for Android Library.
3. Add gcm.jar to libs folder.(will be in the  android_sdk/extras/google/gcm after updating ADT and SDK)

STEP 5. Create A new Project in Android with the following specifications

1) Download gcm-demo-appengine
                https://developers.google.com/appengine/downloads

2) Add API Key as per generated 
 android-sdk -->extras -->google -->gcm-->samples --> gcm-demo-server ---> WebContent -->WEB-INF -->  classes -->api.key
AND
android-sdk/extras/google/gcm/samples/gcm-demo-appengine/src/com/google/android/gcm/demo/server/ApiKeyInitializer.java 

3) Add gcm.jar in Project lib file
            android-sdk -->extras -->google -->gcm-->gcm-client -->dist -->gcm.jar

4) Make the following changes in the application's Android manifest
permissions:
 ```Java
<permission android:name="my_app_package.permission.C2D_MESSAGE" android:protectionLevel="signature" />
<uses-permission android:name="my_app_package.permission.C2D_MESSAGE" />

<!-- App receives GCM messages. -->
<uses-permission android:name="com.google.android.c2dm.permission.RECEIVE" />
<!-- GCM connects to Google Services. -->
<uses-permission android:name="android.permission.INTERNET" /> 
<!-- GCM requires a Google account. -->
<uses-permission android:name="android.permission.GET_ACCOUNTS" />
<!-- Keeps the processor from sleeping when a message is received. -->
<uses-permission android:name="android.permission.WAKE_LOCK" />
 end
    ```
broadcast receiver :
 ```Java
<receiver android:name="com.google.android.gcm.GCMBroadcastReceiver" android:permission="com.google.android.c2dm.permission.SEND" >
 <intent-filter>
   <action android:name="com.google.android.c2dm.intent.RECEIVE" />
   <action android:name="com.google.android.c2dm.intent.REGISTRATION" />
   <category android:name="my_app_package" />
 </intent-filter>
</receiver>
 end
    ```
#Generate an server 
                     Here we have used Tomacat Server 
Refer link to install on mac  : http://www.editrocket.com/articles/tomcat_mac.html
Refer link to install on ubuntu:http://www.mkyong.com/tomcat/how-to-install-tomcat-in-ubuntu/


## To set our project on server 
Copy gcm-demo.war from 
android-sdk -->extras -->google -->gcm-->sample -->gcm-demo-server-->dist -->gcm-demo.war
and paste to 
apache -->webapp

Start server i.e Tomcat 
	on Command line 
 		cd apache-tomcat-7.0
 		cd bin 
 		$ sh startup.sh

Hit the url in browser: http://localhost:8080/gcm-demo

Execute some commands on command prompt :

Refer Link : http://developer.android.com/guide/google/gcm/demo.html

1) android-sdk -->extras -->google -->gcm-->samples --> gcm-demo-server --->
    $ ant war

2)gcm-demo-appengine →
   $ ant -Dsdk.dir=/Users/nachi/Server/appengine-java-sdk runserver -Dserver.host=192.168.0.89

3)android-sdk -->tools
$ ./android update project --name Example --path ~/../../MyDemo/PushNotification-Demo/Example/ --target android-16



Reference Link :
http://developer.android.com/google/gcm/gs.html


