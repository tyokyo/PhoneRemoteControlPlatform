# PhoneRemoteControlPlatform
Android Phone Remote Control minicap

A remote debugging Android mobile platform

Developed with Java language, with the help of minicap and adbkit, it realizes remote click on the mobile screen, ADB connection, obtaining logcat log, uploading and installing app

Stf is commonly used as a classic remote real machine debugging tool, but there are some shortcomings, such as android10 does not support clicking, not stable enough, etc.

And stf is more suitable for internal testing tools, not for remote debugging platforms open to the public.

This platform draws on stf ideas and re-built services designed for remote real machine debugging, using java technology, mysql database, and easier to build and maintain than stf.
 

The platform has been tested on hundreds of Android phones, and the android version supports 4.x to 10.

Installation

1. Configuring the JDK environment, version 1.8

2. Put phoneremotecontrolplatform.war in Tomcat

3. Install MySQL database software, execute installdb.sql under the dbinstall directory to initialize the database, and execute two SQL initialization tables, mobilephoneinfo and parameter

4. Put the resources directory into the directory consistent with the minipath configuration of the database parameter table

5. Install nodejs

6. Execute NPM I - G adbkit on the command line

7. The configuration database adbkitpath is consistent with the directory of the installed \ adbkit.cmd

8. Start Tomcat

9. Browser access http://tomcatip:tomcatport/phoneremotecontrolplatform/devicelist/
