#How to set the run configuration in Webstorm.

This document has defined few steps that you need to follow to setup the run configuration in Webstorm , making your project run directly in the chrome browser.

##The steps to follow are : 
* Launch **Webstorm** and open your project.
* Goto **Run** then **Edit Configurations…**
* Click on **+** sign at the top left corner(Please do not change parameters in the **Defaults**).
* Select **JavaScript Debug**  then **Remote** 
* In **Name** field give the project name (your choice).
In **URL to open:** give the address of **index.html** from you project.
	OR
	you can directly copy the running url from the web browser.

	In my case it is : **http://localhost/MyApp/index.html** 

In Remote URLs of the local files:  give your project URL double click on remote URL field and give this `http://localhost/<project_name>` 

	**in my case it is : http://localhost/MyApp**

Click **Apply** and then **OK**.

That’s all the change you needed to make in the Webstorm , now you just have to add an extension in the **Chrome browser**.			

Open **Chrome**.
In the address bar give this : `chrome://extension/`
Select **Get more extensions**.
Search for **jetBrains IDE Support**
Add the extension and you are Done.

