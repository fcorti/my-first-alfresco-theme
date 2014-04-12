My first Alfresco theme
=======================

Eclipse project creating an Alfresco theme released as AMP and ZIP files.

Using the ANT build file you can create with one click the AMP file and the ZIP file containing your custom Alfresco theme.
This is only an example of Alfresco custom theme, developed with the same layout of the "Green theme" bundled in Alfresco Community Edition and modified as described in this post:
http://fcorti.com/2012/12/31/alfresco-share-custom-theme/

The custom theme packages are stored in the "build" folder.

To deploy the AMP file, you can follow the official tutorials described here:
https://wiki.alfresco.com/wiki/Module_Management_Tool
ATTENTION: The deployment is in the Share WAR, not in the Alfresco WAR!

To deploy the ZIP file: copy it in the Alfresco installation folder and unzip it merging the subfolders.
Of course, first of all, stop Alfresco before everything and start it again after the installation task.

Enjoy your theme!
