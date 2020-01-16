# Apollo-DuerOS
 Apollo-DuerOS is a set of telematics products associated with the Apollo , and there are several open source products at present.
 
## CarLife+ for Android Vehicle 

[CarLife+ for Android Vehicle](https://github.com/ApolloAuto/apollo-DuerOS/tree/master/CarLife-Android-Vehicle) is the implementation of the CarLife+ protocol on the Android platform.

[CarLife+](http://carlife.baidu.com/) is a Smartphone-Integration solution, with which drivers can  share the mobile applications suitable for safe driving conditions on MD (Mobile Device) to HU (Head Unit) through the multi-screen sharing and interaction technology, and use the Touch Screen, Hard Keys, Knob Control and Microphone to control CarLife+. 
![CarLife Screen](CarLife+.jpeg)

All the business logic is on the mobilephone side，and the vehicle side  is primarily responsible for the functions of connection, protocol parsing, video decoding, audio playback and touch events.

CarLife+ mobilephone terminal support iOS and Android platform, vehicle terminal support Android, Linux, WINCE, QNX and other platforms.

CarLife+ currently supports wireless connection. There is no open source code of the wireless connection part. Please contact us if you are interested in embedding wireless CarLife+ in your projects. If you are willing to integrate wireless CarLife+ into a mass production project, we have to check authenticity of the project and will provide you with the spec and sample code.

## CarLifeVehicleLib
[CarLifeVehicleLib](https://github.com/ApolloAuto/apollo-DuerOS/tree/master/CarLife-Vehicle-Lib) is a C++ based cross platform dynamic library, which realizes the function of channel establishment, data sending and receiving, protocol parsing and packing in HU CarLife. Using this library can speed up the development of CarLife in HU.


## DuerOS Launcher
Launcher is the interface of the first user graphical interaction of the Android terminal,is the start of the installation of other applications on the terminal entrance(Telephone, radio, and so on need to be connected to app).
![Launcher Screen](Launcher.jpeg)

### [DuerOS Launcher](https://github.com/ApolloAuto/apollo-DuerOS/tree/master/DuerOS-Launcher) Features:
1. For the driving scene design, using lightweight, scientific sense of the UI design

2. The home page aggregated voice, maps, music and other entrances, the car scene is more convenient to use

## DSP Solution for Apollo DuerOS
[The  DSP solution](https://github.com/ApolloAuto/apollo-DuerOS/tree/master/DSP-Solution-For-DuerOS) includes two parts: front-end signal acquisition and voice signal processing.
![DSPSolution](DSPDesign.png)
Front-end signal acquisition is completed through a set of MIC array (2~3 MIC), while the voice signal processing is achieved by DSP. The DSP chips embedded into the motherboard of the vehicle would work on echo’s noise cancellation and directional voice pick-up, and then convey the processed signal to the main CPU layer, and finally the signals would flow into the Baidu Voice ASR Engine.

## DuerOS Auto Spec
[DuerOS Auto Spec](https://github.com/ApolloAuto/apollo-DuerOS/tree/master/DuerOS-Auto-Spec) is the integration guide of DuerOS Auto,including the integration of the DuerOS Auto software and hardware requirements, the access process description,  functions and  interfaces description, the test and acceptance process ,etc. The partner OEM can carry out DuerOS Auto according to this document.
