My first Alfresco theme
=======================

Eclipse project creating an Alfresco theme released as AMP and ZIP files.

Using the ANT build file you can create with one click the AMP file and the ZIP file containing your custom Alfresco theme.
This is only an example of Alfresco custom theme, developed with the same layout of the "Green theme" bundled in Alfresco Community Edition and modified as described in this post:
http://fcorti.com/2012/12/31/alfresco-share-custom-theme/

The custom theme packages are stored in the "build" folder.

How to package the theme
=======================

Open the ANT view in Eclipse clicking: Window -> Show view -> ANT.

Add the build file pressing the plus ant button in the ANT view.

The build file to add is stored in the Java project with the name 'build.xml'.

Press the 'Run' button in the ANT view.

Refresh the content of the 'build' folder of the project and check for the AMP file and the ZIP file.

How to deploy the AMP file
=======================

Open a terminal and go to the folder where Alfresco is installed (for example: '/opt/alfresco-4.2.f').

Stop Alfresco with the command: ./alfresco.sh stop

Copy the AMP file from the 'build' folder of the project in the 'amps-share' folder.

Go to the bin subfolder and run the command: ./apply_amps.sh

Go back to the Alfresco installation folder and start Alfresco again with the command: ./alfresco.sh start

Once Alfresco is started, open a browser with the URL 'http://IP:PORT/share', login as administrator and access to 'Admin tools' item in the menu.

In 'Applications', change the theme to your custom theme.

That's all!

How to deploy the ZIP file.
=======================

Open a terminal and go to the folder where Alfresco is installed (for example: '/opt/alfresco-4.2.f').

Stop Alfresco with the command: ./alfresco.sh stop

Copy the ZIP file from the 'build' folder of the project in the folder and unzip it, merging the subfolders with the content.

Start Alfresco again with the command: ./alfresco.sh start

Once Alfresco is started, open a browser with the URL 'http://IP:PORT/share', login as administrator and access to 'Admin tools' item in the menu.

In 'Applications', change the theme to your custom theme.

That's all!
