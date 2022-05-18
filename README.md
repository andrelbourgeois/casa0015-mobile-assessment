# CroissAcq

## Description
The intent of this project was to develop a mobile app using Flutter and Dart that would allow a user to press a button and be routed towards the croissant nearest to their location.

## Key Assumptions
The major assumption being made within this project is that every bakery or cafe will have a croissant. As it would be impossible (or near enough) to actually determine which locations bake croissants and which locations still have croissants in stock, the best way to lead someone to their probable closest croissant would be to route them to the bakery closest to their location. Therefore, this project aims to to just that - route users to their closest bakery or cafe in order to acquire a croissant.

## Key Packages Used
[**firebase_auth 3.3.17**](https://pub.dev/packages/firebase_auth)

Used for the purpose of authentication users, links with firebase within Google Cloud Platform

[**google_maps_flutter 2.0.2**](https://pub.dev/packages/google_maps_flutter)

Used in conjunction with Google Maps API in order to host a map in-app

[**flutter_polyline_points 0.2.6**](https://pub.dev/packages/flutter_polyline_points)

This package contains functions to decode google encoded polyline string which returns a list of co-ordinates indicating route between two geographical position

[**geolocator 8.2.1**](https://pub.dev/packages/geolocator)

A Flutter geolocation plugin which provides easy access to platform specific location services

[**geocoding 2.0.4**](https://pub.dev/packages/geocoding)

Geocoding is the computational process by which a physical address is converted into geographic coordinates. This package provides geocoding and reverse geocoding features. 

## Process
**Develop App Prototype**

Before beginning this build I protoyped CroissAcq on [Figma](https://www.figma.com) to get an idea of how I wanted the app to look and feel for the user.
![Figma App Prototype](https://user-images.githubusercontent.com/33913141/169050269-80cea902-d18c-4040-b173-f8862cb0ab56.png)


**Set Up Flutter App**

Following the prototype, I set up an initial Flutter application

**Implement Navigation and App Hierarchy**

Once the Flutter application was set up, I wanted to implement more screens. This also entailed deciding in what order to display screens and deciding how best to navigate throughout this hierarchy. I decided that a drawer menu would be best to faciliate navigation, and that subsequent screens should branch out from the home screen. Throughout this process, I realized that the code for the drawer menu would need to be replicated for every screen it was needed on. Therefore, I decided to rewrite it as a standalone function which I can call to each screen, instead of rewriting code.

**Implementing Firebase and Authorization**

Once I had a few pages laid out, I wanted to handle user information handling and authorization. Using Firebase - various code and tutorials referenced below - I implemented welcome, registration, and login screens to obtain user information (email and password) which is subsequently stored within a Firebase project. This project and database are then used to match user information together and allow or deny access to the rest of the app. A profile screen was also implemented which retrieves user information (email) from Firebase and displays it for the logged in user. This screen can be accessed by tapping the avatar circle at the top of the drawer menu. Additionally, the profile screen allows the user to log out.

**Implementing Mapping Functionality**

talk about setting up google maps API, and then using reference material to implement routing features

## To Do
- Make colouring consistent
- Implement avatar image in drawer menu and profile screen
- Isolate mapping functions into a separate file
- Utilize routing features to create the "FIND ME A CROISSANT" button
- Implement validation error handling for authorization

## License
MIT License

Copyright (c) André Bourgeois andrelbourgeois@gmail.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.




## Use this README File 

Use this section to show us what your Mobile App is about.   Include a Screenshot to the App, link to the various frameworks you've used. Include your presentation video here that shows off your Mobile App.   Emojis are also fun to include 📱 😄

Look at some other Flutter Apps online and see how they use there README File.  Good examples are:

- https://github.com/miickel/flutter_particle_clock
- https://github.com/Tarikul711/flutter-food-delivery-app-ui    
- https://github.com/mohak1283/Instagram-Clone


## Include A Section That Tells Developers How To Install The App

Include a section that gives intructions on how to install the app or run it in Flutter.  What versions of the plugins are you assuming?  Maybe define a licence
