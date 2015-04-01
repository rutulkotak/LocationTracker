# LocationTracker
Track Location using Fused provider and GoogleMap

Goal
===============
This Android tutorial will walk you through to create a location tracker using Android location API and Google maps services.
This deals mainly with two areas, using the location API to continuously get the user location and showing that lat-long position in GoogleMap

Helps to understand:
1. Android location using fused provider
2. Google Maps Android API v2
3. Markers on Map

Prerequisite to user Google Maps API
===============
1. Create project in Google Console https://cloud.google.com/console/project
2. Then go to menu “APIs & auth –> APIs” and switch on “Google Maps Android API v2”
3. Create SHA1 Android key by running the following command in cmd prompt (you should have JDK installed and PATH setup).
keytool -list -v -keystore "%USERPROFILE%\.android\debug.keystore" -alias androiddebugkey -storepass android -keypass android
4. Grab SHA1 value from above cmd prompt and go back to Google Console to create Android API key.
   Go to menu “APIs & auth –> Credentials” in ‘Public API access’ click create new Key button. 
   Then used the SHA1 key generated and the android application package to create and get the Android API key.
5. Add Google Play Services to project dependency. Just add the following in Gradle dependencies.
   compile 'com.google.android.gms:play-services:6.5.87'
