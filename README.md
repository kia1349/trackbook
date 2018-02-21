README
======

Trackbook - Movement Recorder for Android
-----------------------------------------

**Version 1.1.x ("Sheep")**

Trackbook is a bare bones app for recording your movements. Trackbook is great for hiking, vacation or workout. Once started it traces your movements on a map. The map data is provided by [OpenStreetMap (OSM)](https://www.openstreetmap.org/).

Trackbook is free software. It is published under the [MIT open source license](https://opensource.org/licenses/MIT). Trackbook uses [osmdroid](https://github.com/osmdroid/osmdroid) to display the map, which is also free software published under the [Apache License](https://github.com/osmdroid/osmdroid/blob/master/LICENSE). Want to help? Please check out the notes in [CONTRIBUTE.md](https://github.com/y20k/trackbook/blob/master/CONTRIBUTE.md) first.

Install Trackbook
-----------------
You can install it via Google Play and F-Droid - or you can go and grab the latest APK on [GitHub](https://github.com/y20k/trackbook/releases).

[<img src="https://play.google.com/intl/de_de/badges/images/generic/en_badge_web_generic.png" width="192">](https://play.google.com/store/apps/details?id=org.y20k.trackbook)

[<img src="https://cloud.githubusercontent.com/assets/9103935/14702535/45f6326a-07ab-11e6-9256-469c1dd51c22.png" width="192">](https://f-droid.org/repository/browse/?fdid=org.y20k.trackbook)

How to use Trackbook
--------------------
### Start recording movements
Press the big blue button to start recording your movements. Trackbook will continuously drop markers onto the map.

### Stop recording movements
To stop your recording press the big blue button again or use the stop button in the Trackbook's notification. You can look at the recorded movements on the map afterwards.

### Save last recording
Stop the recording and then tap again on the big blue button. It will offer an option to "Save and Clear". Trackbook stores saved recordings as plaintext JSON files in the directory `/Android/data/org.y20k.trackbook/files/tracks`.

### Clear main map
Stop the recording and then tap again on the big blue button. Chose the option "Clear", if you just want to clear the map without saving your recording.

### Statistics and Last Tracks
Peek into Trackbook's notification to see the distance and duration of your current recording. Switch to the "Last Tracks" view to review your last recordings - up to 25 tracks. Pull up the statistics to see distance and duration of that recording, as well as the steps taken.

### GPX Export
Saved recordings can be exported as GPX ([GPS Exchange Format](https://en.wikipedia.org/wiki/GPS_Exchange_Format)) from the "Last Tracks" view. Just tap the export icon next to the track selection menu.

### How does Trackbook measure distance?
Trackbook calculates the distance between markers and adds them up.

Which Permissions does Trackbook need?
--------------------------------------
### Permission "INTERNET"
Trackbook needs to download map data from OpenStreetMap servers and therefore needs access to the internet.

### Permission "ACCESS\_NETWORK\_STATE" and "ACCESS\_WIFI\_STATE"
Trackbook uses [osmdroid](https://github.com/osmdroid/osmdroid/) to draw its maps. osmdroid needs to know the current state of your device’s connectivity - see [Prerequisites](https://github.com/osmdroid/osmdroid/wiki/Prerequisites).

### Permission "ACCESS\_COARSE\_LOCATION" and "ACCESS\_FINE\_LOCATION"
Trackbook needs accurate GPS location data to be able to record your movements. If the GPS data is not available or not accurate enough Trackbook uses location data from cell tower and WiFi triangulation.

### Permission "VIBRATE"
Tapping and holding some controls will toggle a tiny vibration (force feedback).

### Permission "WRITE\_EXTERNAL\_STORAGE"
Trackbook uses [osmdroid](https://github.com/osmdroid/osmdroid), which caches map tiles on Android's external storage. You can find the map cache in the `osmdroid` folder on the top level of the user-facing file system.

Screenshots (v1.1)
------------------
[<img src="https://user-images.githubusercontent.com/9103935/34250760-22dd45e8-e63e-11e7-8e78-9d928470e92a.png" width="240">](https://user-images.githubusercontent.com/9103935/34250760-22dd45e8-e63e-11e7-8e78-9d928470e92a.png)
[<img src="https://user-images.githubusercontent.com/9103935/34250761-22ff00b6-e63e-11e7-974a-47c238d477e0.png" width="240">](https://user-images.githubusercontent.com/9103935/34250761-22ff00b6-e63e-11e7-974a-47c238d477e0.png)

[<img src="https://user-images.githubusercontent.com/9103935/34250762-2316aa90-e63e-11e7-9bcb-a230467fc192.png" width="240">](https://user-images.githubusercontent.com/9103935/34250762-2316aa90-e63e-11e7-9bcb-a230467fc192.png)
[<img src="https://user-images.githubusercontent.com/9103935/34250763-232f7714-e63e-11e7-92bf-1fda9442e443.png" width="240">](https://user-images.githubusercontent.com/9103935/34250763-232f7714-e63e-11e7-92bf-1fda9442e443.png)
