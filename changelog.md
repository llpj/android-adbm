Change Log
==========
#### 1.0.2

###### Bugfixes:

* Very rarely the service got called with null action, and because of it crashed the service

#### 1.0.1

###### Bugfixes:

* Fixed a crash that happens if you haven't saved any WiFi networks in the system, when you open the configuration screen for WiFi networks in settings

#### 1.0.0

Released as open source

#### 0.9.9

You should reset your preferences for this update from the preferences screen.

###### Features:

* Added a status to show if we have wakelock or not

###### Bugfixes:

* Tidy up for the strings, also added new time intervals for the preferences screen
* Hopefully fixed the issue with AlarmManager holding the CPU awake, even if we don't have a wake lock acquired


#### 0.9.8

###### Bugfixes:

* Fixed the wake lock issues on some occasions

#### 0.9.7

###### Bugfixes: 

 Sometimes the service doesn't start fast enough so it cannot bind the service in time to request update, and it results in an crash

#### 0.9.6

###### Features:

* You can toggle the ADB state by touching the image in the notification bar

#### 0.9.5

###### Bugfixes:

* Doesn't release wakelock always

#### 0.9.4

###### Features:
* Added an option to keep screen on while the service is running
* Added an option to wake the screen when new package is installed if the keep screen functionality is not on

###### Permission:
* android.permission.WAKE_LOCK
  Used to wake up the screen on new package install, or to keep the screen on while the ADB service is on

#### 0.9.1

###### Bugfixes:
* Fixed a crash that occurs sometimes when starting the service

#### 0.9

###### Features: 
* Added a Widget

###### Bugfixes:
* Various optimizations and bugfixes

#### 0.8.4

###### Features: 
* Added About menu
* Added Change Log menu

###### Bugfixes:
* Various optimizations and bugfixes

#### 0.8.3

###### Features:
* Added the ability to make the notification permanent or be able to clear it

###### Bugfixes:
* ADB Network status not updating properly

#### 0.8.2

###### Features:
* Added new icon for the states, now it has different icons for various states.
  White overlay: No WiFi connections
  Sky blue overlay: WiFi connection available but no connections
  Yellow overlay: WiFi connected, and ADB is running in network state

###### Bugfixes:
* Sometimes the DISCONNECT event didn't update the notification bar

#### 0.8.0 - Initial release

###### Features:
* Easy control and access details from notification bar
* Auto connect on saved WiFi networks
* Auto start on boot, you can select if you want to or not from the preferences screen
* Automatically switch between USB and NETWORK when you disconnect/connect from/to WiFi
* Configurable service management