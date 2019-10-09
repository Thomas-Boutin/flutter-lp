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

This will give you the secrets required to call the API

### Step 3 : Create a new project

Create a new project using your IDE or the flutter CLI

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

- Take a look at the [ex4](../ex4) to find examples of Navigation, Click handling, etc
- [Venues API link](https://developer.foursquare.com/docs/api/venues/search)
- Dart has a packagage manager (like NPM)
