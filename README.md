Ubuntu-Android-CMD
==================

To Run Emulator
---------------
<pre>
export LD_LIBRARY_PATH="/home/nazmul/Android/Sdk/tools/lib64:$LD_LIBRARY_PATH"
cd /home/nazmul/Android/Sdk/tools
~/Android/Sdk/tools$ ./emulator64-x86 -avd <device name> -gpu on
</pre>
or
--
######install apk in command line
<pre>
adb install <path_to_your_bin>.apk
adb -s emulator-5554 install path/to/your/app.apk
adb -d install path/to/your/app.apk
</pre>

PLAYSTORE + Google Play Service
-------------------------------
<pre>
/Android/Sdk/tools$ ./emulator64-x86 -avd Kitkat -partition-size 566 -no-audio -no-boot-anim
cd Android/Sdk/platform-tools
platform-tools$ adb shell mount -o remount,rw -t yaffs2 /dev/block/mtdblock0 /system
platform-tools$ adb shell chmod 777 /system/app
platform-tools$ adb push /home/nazmul/Downloads/GoogleLoginService.apk /system/app/.
platform-tools$ adb push /home/nazmul/Downloads/GoogleServicesFramework.apk /system/app/.
platform-tools$ adb push /home/nazmul/Downloads/Phonesky.apk /system/app/.
platform-tools$ adb shell rm /system/app/SdkSetup*
</pre>

Install LAMP
------------

https://help.ubuntu.com/community/ApacheMySQLPHP
or
<pre>
$ sudo apt-get update
$ sudo apt-get install lamp-server^
</pre>

Install Grameenphone Modem IN LINUX
-----------------------------------

######Save the PCL_Bengle file to home or Download Directory
######Go to that location in terminal
##run the command 
<pre>
sudo ./install.sh
install apk in command line
adb install <path_to_your_bin>.apk
adb -s emulator-5554 install path/to/your/app.apk
adb -d install path/to/your/app.apk
</pre>

ImortantLinks
-------------
#####Sliding photo from Json
http://androidopentutorials.com/
#####Google Play Service In Emulator
#####windows
http://www.securitylearn.net/2013/08/31/google-play-store-on-android-emulator/
#####Linux
http://stackoverflow.com/questions/11154222/google-play-on-android-4-0-emulator
#####Add toolbar to an app
http://developer.android.com/training/appbar/setting-up.html
#####Navigation indecator Color change
http://stackoverflow.com/questions/31626488/change-the-color-of-navigation-drawer-indicator-icon
#####Different Matarial Animation
https://github.com/lgvalle/Material-Animations
#####SettingActivity PreferencesActivity
https://github.com/AndroidDeveloperLB/MaterialPreferenceLibrary
#####Different payment methods
http://www.freelancerstory.com/

Install Avro In Linux
---------------------
http://linux.omicronlab.com/ubuntu_14.04.html
