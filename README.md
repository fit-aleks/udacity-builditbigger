# Gradle for Android and Java Final Project

The finished app consists of four modules. A Java library that provides jokes, a Google Could Endpoints
(GCE) project that serves those jokes, an Android Library containing an
activity for displaying jokes, and an Android app that fetches jokes from the
GCE module and passes them to the Android Library for display.

### Components

* Project contains a Java library for supplying jokes
* Project contains an Android library with an activity that displays jokes passed to it as intent extras.
* Project contains a Google Cloud Endpoints module that supplies jokes from the Java library. Project loads jokes from GCE module via an async task.
* Project contains connected tests to verify that the async task is indeed loading jokes.
* Project contains paid/free flavors. The paid flavor has no ads, and no unnecessary dependencies.

### Behavior

* App retrieves jokes from Google Cloud Endpoints module and displays them via an Activity from the Android Library.

### Other Components

Also app fully implements following items.

* The free app variant displays interstitial ads between the main activity and the joke-displaying activity.
* The app displays a loading indicator while the joke is being fetched from the server.
* The root build.gradle file contains a task that will start up the GCE development server, run all Android tests, then shutdown the development server.

## Screens

<img src="https://github.com/fit-aleks/udacity-builditbigger/blob/master/art/MainScreen.png" alt="" width="272" height="465" />
<img src="https://github.com/fit-aleks/udacity-builditbigger/blob/master/art/JokeText.png" alt="" width="272" height="465" />
<img src="https://github.com/fit-aleks/udacity-builditbigger/blob/master/art/JokeImage.png" alt="" width="272" height="465" />
