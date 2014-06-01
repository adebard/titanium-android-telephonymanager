titanium-android-telephonymanager
=================================

Titanium android module for TelephnyManager


Building:

See the Titanium documentation for how to compile modules: 
http://docs.appcelerator.com/titanium/3.0/#!/guide/Android_Module_Development_Guide

Install:

See the Titanium documentation for how to install modules into project: 
http://docs.appcelerator.com/titanium/3.0/#!/guide/Using_a_Module

Usage:

var tm = require('com.adebard.telephonymanager');

tm.getPhoneNumber();

Then we need to add user permission into tiapp file 
    
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>

Note: so far some people have conflict about different behavior of  output.
There are reports that some SIMs cause this method to return null.

Some phone companies do not record the telephone number in the SIMs.