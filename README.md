# Cordova-Javascript

Make sure npm is installed on your machine. NPM is installed along with node.js

Goto www\scripts folder in command prompt and type
npm install angular - this may not install the package to the desired folder. Run the below.
npm install angular --prefix .

This will install angular in to the node_modules folder. In the dependency under npm you can see that angular is installed.

load your angular script into the html. Make sure the index.js is the last one in the list. If not then it may raise an object not found issue when accessing angular.


locFinder is the angular module name. The module which we have created in index.js

ng-controller specifies the controller.
ng-click defines the click handler.

<div ng-app="locFinder" ng-controller="locFinderController as finder">
            <div>
                <button class="btn" ng-click="finder.getLocation()">Find my location</button>
                <div>your location is {{lat}}, {{long}}</div>
            </div>


Open config.xml, this will open a configuration UI. Enable geolocatin module.
