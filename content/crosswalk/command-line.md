/*
Title: Crosswalk Command Line
Sort: 1
*/

To Try This
===========

I am listing my steps for your reference:

1.         Download latest Cordova bundle of Crosswalk-6 beta version

a)         x86: https://download.01.org/crosswalk/releases/crosswalk/android/beta/6.35.131.11/x86/crosswalk-cordova-6.35.131.11-x86.zip

b)         ARM: https://download.01.org/crosswalk/releases/crosswalk/android/beta/6.35.131.11/arm/crosswalk-cordova-6.35.131.11-arm.zip

2.         Open a console and export ADT path

a)         E.g. export PATH=${PATH}:/path_to_adt/sdk/tools/:/path_to_adt /sdk/platform-tools/

3.         Create app template

a)         E.g. ./crosswalk-cordova-6.35.131.11-arm/bin/create pdf org.example.pdf pdf

4.         Edit res/xml/config.xml, set <content src="http://mozilla.github.io/pdf.js/web/viewer.html" />

5.         ./cordova/build and ./cordova/run


This is Not Working
==============================
Not working, I guess becouse of windows path / \ confusion, need to test on linux/ios

(https://crosswalk-project.org/#documentation/cordova/migrate_an_application)[https://crosswalk-project.org/#documentation/cordova/migrate_an_application]

rm -Rf platforms/android/CordovaLib/*

cp -a /d/js/crosswalk-cordova-6.35.131.7-x86/framework/* platforms/android/CordovaLib/

cp -a /d/js/crosswalk-cordova-6.35.131.7-x86/VERSION platforms/android/

from cmd:

d:

cd d:\js\ionic03_cw_commandline

cd platforms\android\CordovaLib

android list targets

android update project --subprojects --path . --target 4

bash:

cd platforms/android/CordovaLib/

ant debug