# Exoplayer Test

This app is for testing mp4, dash, live streaming(RTMP).


## Trouble shooting page

https://exoplayer.dev/troubleshooting.html


### Fixing “Cleartext HTTP traffic not permitted” errors

This error will occur if your app requests cleartext traffic (e.g., http:// rather than https://) when its Network Security Configuration does not permit it. If your app targets Android 9 (API level 28) or later, cleartext traffic is disabled by the default configuration.

If your app needs to work with cleartext traffic (e.g., to stream media over http://) then you need to use a Network Security Configuration that permits it. Please see Android’s network security documentation for details. To enable all cleartext traffic, you can simply add android:usesCleartextTraffic="true" to the application element of your app’s AndroidManifest.xml.
