A Java application for face recognition under expressions, occlusions and pose variations.

Description:
This is a prototype with the goal of improving recognition accuracy and reliability under un-cooperative scenarios like expressions, occlusions (obstacles like spectacles) and pose variations (<60deg).

The project is tested with Bosphorous Database (http://bosphorus.ee.boun.edu.tr/default.aspx).

Running the project:
Install latest version of JDK.

Install NetBeans.

Go to Control Panel->Add or Remove Programs(Uninstall Programs) and check any other databases are installed (e.g. Microsoft SQL or simply MySQL). If so, uninstall all.

Install Microsoft Visual C++ Redistributable Package (vcredist_x86.exe).

Intall WAMP Server and start it.

Open NetBeans and create a new Java project. Delete the default package created. (For example, if the project name is abc, then NetBeans automatically creates a package with the same name along with .java file. Delete the complete package in Source Packages section )

Open the code and copy full "src" folder(Parent folder of all .java files) and paste it on Source Packages in NetBeans.

Now right click on Libraries and choose Add JAR/Folder option and open the "libs" folder that came with code. Select all(CTRL+A) and click Open.

Copy all .dll files came with code in the "dll" folder to C:\Windows folder [ONLY FOR 32 BIT SYSTEMS].

Install Java 3D API(java3d_1_5...exe).

Go to C:\Program Files\Java\Java3D\bin and copy all DLLs to C:\Windows [ONLY FOR 64 BIT SYSTEMS].

Open System Tray->Wamp Server green icon->Left Click->MySQL->MySQL Console. Press Enter. You should see mysql> prompt.

Enter the following commands:

 
 create database 3dface;
 use 3dface;
 create table users(UserName varchar(30),Email varchar(50),Phone varchar(10),Password varchar(20));
 exit;
 
Again open system tray->Wamp green icon left click->phpMyAdmin. Browser will be opened. Database list on left side. Click on "3dface". You can see "users" table and get confirmed with the same.

Run the project.# face-recognition
