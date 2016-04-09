# WebRTC Android Basic Tutorial
>Using the DataChannel to communicate between two peers on one Android device

As I was searching for tutorials using WebRTC on native Android I found many that either taught you to use a specific SDK or taught 
you only the basics of Video/Audio chat clients. What I really wanted was a tutorial that taught you the basics of using the DataChannel
on Android to transmit data between peers. Since I found none, I decided to make one.

Following this tutorial or looking through the code you will learn how to use the PeerConnection API to create two peers inside an Android
and exchange data between using the DataChannel. This will thus give you the basics to implement more complicated and interesting applications.

###Getting Started
Before developing Android apps that use native WebRTC you need the compiled code. [WebRTC.org](https://webrtc.org/native-code/android/) offers
a barebones guide to obtaining the compiled Java code. But a simpler way to get this code is to use the library offered by [IO.Pristine](http://mvnrepository.com/artifact/io.pristine/libjingle).
This is done by placing the following inside `build.gradle` for the app.
```
compile 'io.pristine:libjingle:_version_@aar'
```
Where `_version_` represents the current version of the library. The current working version is `11139`. (04/09/2016)
  
###How it works


