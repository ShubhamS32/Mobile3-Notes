
## Setup Process for Monkey Talk

*	Monkey Talk can be downloading from the below address:

	`http://www.gorillalogic.com/testing-tools/monkeytalk/download`

*	Pre-requisit for installing Monkey Talk Agent:

*	For installing the Monkey Talk Android Agent, first we need to convert Android project into AspectJ.

*	For doing so, we need to configure AJDT in Eclipse by following steps:

*	Eclipse> Help> Install New Software > Click on Add…

*	In `Add Repository` popup:

	Name: `AJDT`

	Location: `http://download.eclipse.org/tools/ajdt/37/update`

*	Click Ok. It will configure the AJDT with Eclipse.


## Steps to install MonkeyTalk Android Agent

	1. Open your android project in eclipse.

	2. Convert your android project in AspectJ .

	3. Create a folder in your android project named as `libs` ,  if you don’t already have one.

	4. Copy the `MonkeyTalk-agent.jar` file in libs folder.

	* `MonkeyTalk-agent.jar` can be found in the `agents` folder in the MonkeyTalk package you downloaded earlier. The exact name of the jar 			might vary depending on the version, but it should always start with “MonkeyTalk-agent”.

	5. Now add this MonkeyTalk jar file to aspect path:

	Right click on MonkeyTalk-agent.jar

	Go to  AspectJ Tools

	Click on  Add to Aspectpath

	6. Update your AndroidManifest.xml to include the following two permissions:

		android.permission.INTERNET
		android.permission.GET_TASKS

	<uses-permission android:name=”android.permission.GET_TASKS” />

	<uses-permission android:name=”android.permission.INTERNET” />

	*You can find Androidmanifest.xml file under res folder of your android project.*

	7. Update the project properties (right-click on the project > Properties > Java Build Path), 

		select the Order and Export tab, and 
		check the checkbox next to the AspectJ Runtime Library to export it.

	8. Deploy your application to an Android device or emulator.

	Right click on Android project

	Choose `Run as` option and then `Android Application`



