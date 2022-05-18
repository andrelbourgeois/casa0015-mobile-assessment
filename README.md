# CroissAcq

## Description
The intent of this project was to develop a mobile app using Flutter and Dart that would allow a user to press a button and be routed towards the croissant nearest to their location.

## Key Assumptions
The major assumption being made within this project is that every bakery or cafe will have a croissant. As it would be impossible (or near enough) to actually determine which locations bake croissants and which locations still have croissants in stock, the best way to lead someone to their probable closest croissant would be to route them to the bakery closest to their location. Therefore, this project aims to to just that - route users to their closest bakery or cafe in order to acquire a croissant.

## Key Packages Used
[**firebase_auth**](https://pub.dev/packages/firebase_auth)

Used for the purpose of authentication users, links with firebase within Google Cloud Platform

[**google_maps_flutter**](https://pub.dev/packages/google_maps_flutter)

Used in conjunction with Google Maps API in order to host a map in-app

[**flutter_polyline_points**](https://pub.dev/packages/flutter_polyline_points)

This package contains functions to decode google encoded polyline string which returns a list of co-ordinates indicating route between two geographical position

[**geolocator**](https://pub.dev/packages/geolocator)

A Flutter geolocation plugin which provides easy access to platform specific location services

[**geocoding**](https://pub.dev/packages/geocoding)

Geocoding is the computational process by which a physical address is converted into geographic coordinates. This package provides geocoding and reverse geocoding features. 

## Process
**Develop App Prototype**

insert explanation of prototpe and figma links, why prototyping first helped me

**Set Up Flutter App*

words

**Implement Navigation and App Hierarchy**

talk about implementing different screens, drawer menu, and turning drawer menu into a function to be called to each screen instead of rewriting so much code

**Implementing Firebase and Authorization**

talk about setting up firebase, and bring functionality into app, using reference code to create welcome, registration, and login pages, setting up a profile screen to retrieve user data, and implementing signout

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
