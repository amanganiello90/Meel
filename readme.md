# MealDate

this is the latest front-end of our app 'MealDate' for Yale CPSC 539 Software Engineering.

#### Update Log

```
2019-03-09 23:48:00: FB login temporarily disabled
2019-03-09 22:53:00: allow facebook login
2019-03-09 17:28:00: bugs fix
2019-02-25 13:54:00: add login authentication
2019-02-24 00:32:00: add static login page
2019-02-23 01:00:00: app created
```

## Quick Setup

#### 1, Node.js

```bash
# Check if you have `node.js` 
# ([download_link](https://nodejs.org/en/download/))
node --version
```

#### 2, Ionic & Angular

```bash
# This comes with all of the Ionic components 
# and Angular specific services and features.
npm install -g ionic 
npm install -g @angular/cli
npm install @ionic/angular@latest --save
```

#### 3, Cordova(iOS Native Support)

```bash
# First, download and `cd` to this project
# then run the following command
npm i -g cordova
npm install -g ios-sim
npm install -g ios-deploy
npm install @ionic-native/http --save
ionic cordova plugin add cordova-plugin-advanced-http
ionic cordova plugin add cordova-plugin-facebook4
ionic cordova plugin add cordova-sqlite-storage
ionic cordova prepare ios
```

## Build & Run

#### 1, iOS Emulation(simplified)

```bash
# build and test params are already writen in local script.
npm run emulate-live
```

#### 2, Web Emulation

**WARNING:** this will not be supported in future due to the incorporation of native calls.

```bash
ionic serve -l
```

#### 3, iOS Device

```bash
# Firt Run this to compile
ionic cordova prepare ios

# Then, open Xcode. Use File » Open and locate the app. Open the app platforms/ios directory
# 2, Plug in your iphone into your PC
# 3, Select Buikd » and select your device to run the app!	
```

#### 4, ~~Android Device~~

Not implemented yet.