# Project: Create your own activities search engine app

This project has 2 parts:

- The development of the Flutter app
- The writing of a report

## Flutter app development

### Step 0 : Check your requirements

- Open a console and type

```bash
flutter doctor
```

- Check that you have at least one IDE with the Flutter plugin and an available device / emulator

### Step 1 : Create an account on Foursquare

- We'll use the Foursquare API to browse the venues.
- Create a developer account on their [website](https://developer.foursquare.com)

### Step 2 : Create an app in your developer account

- This will give you the secrets required to call the API
- You can provide whatever you want as a website URL

### Step 3 : Create a new project

- Create a new project using your IDE or the flutter CLI
- Be careful : you should put your secrets in a gitignored file.
- For instance : create a file "env.dart" in lib/
- Define one constant for each secret
- Add en entry in the .gitignore for this file
- [Don't forget to add the internet permission in android/app/AndroidManifest.xml](https://stackoverflow.com/questions/2378607/what-permission-do-i-need-to-access-internet-from-an-android-application)


### Step 4 : Develop the app

The app must have atleast 2 screens

#### Screen #1 : Venues search and list

This screen must at least :

- Have one input to let the user choose the location of his search
- Have one input to let the user choose what he'd like to find as venue
- Have one submit button to let the user perform the search
- Have one list which will contain the results of the query
  - Each result must have a title and an icon
  - When a result is clicked, the app performs a navigation to the screen #2

#### Screen #2 : Venue's details

This screen must at least :

- Show the venue's title in the top app bar
- Give further details on the venue
- Show some pictures of the place (if some exist)
- Show some comments on the place (if some exist)
- Have an input offering the user to open the destination in google maps
  - On click, the browser opens up with the web version of google maps at the given destination

## Report

Write a short report (1-2 pages) which answers this question :

- According to you, can we use Flutter for a business app?

## Tips & Tricks

- Parsing tool : [quicktype](https://app.quicktype.io/)
- Take a look at the [ex4](../ex4) to find examples of Navigation, Click handling, etc
- [HTTP call](https://flutter.dev/docs/cookbook/networking/fetch-data)
- [Venues API link](https://developer.foursquare.com/docs/api/venues/search)
- [Dart has a package manager (like NPM)](https://pub.dev/)
- To get the icons : 
```
Pieces needed to construct category icons at various sizes.
Combine prefix with a size (32, 44, 64, and 88 are available) and suffix.
Example https://foursquare.com/img/categories/food/default_64.png.
To get an image with a gray background, use bg_ before the size.
Example : https://foursquare.com/img/categories_v2/food/icecream_bg_32.png.
```
- To get the pictures :
```
To assemble a photo URL, combine the response’s prefix + size + suffix.
Ex: https://igx.4sqi.net/img/general/300x500/5163668_xXFcZo7sU8aa1ZMhiQ2kIP7NllD48m7qsSwr1mJnFj4.jpg

size can be one of the following, where XX or YY is one of 36, 100, 300, or 500.
```
- There is [an endpoint for the venue's pictures](https://developer.foursquare.com/docs/api/venues/photos)

- There is [an endpoint for the venue's comments](https://developer.foursquare.com/docs/api/venues/tips)
