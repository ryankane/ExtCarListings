# CarListingApp: A DeftJS Example Application

## Preamble

This application is an extension of the [Car Listings](https://github.com/SenchaArchitect/CarListings) by GitHub user [philstrong](https://github.com/philstrong). The original application did not use IoC, so I added Deft JS into the application by following the [Pheonix Application](https://github.com/deftjs/Examples/tree/master/phoenix-example-app) by GitHub user [brian428](https://github.com/brian428).

## Introduction

This example application simulates a disaster recovery scenario tool. If this were real, the idea would be to allow decision-makers to set up plans for different disaster scenarios and weigh their costs and benefits. It uses client storage for persistence, to avoid the need for users to have an application server running. 

While this makes it as easy as possible for people to run the app, it does have its limitations. The primary one being: server-side logic should really handle updating and deleting associations, along with algorithms to evaluate each scenario, its impacts, and determine its effectiveness. As a result, generating these values is simulated in this application. The point here isn't to build complex, production-worthy algorithms to analyze disaster mitigation plans. It's to show how a realistic DeftJS application is designed.

## Screenshot

![Application screenshot](ExtCarListings.png)

## Application Highlights

The application demonstrates a wide range of DeftJS features, including:

* An architecture which uses models, views, ViewControllers, services, and stores
* Application configuration class (AppConfig)
* Application initialization and data loading at startup
* Injector and dependency provider setup
* Dependency injection (with inherited injections)
* Use of ViewControllers to handle view events and encapsulate UI-related logic
* Use of the Observe feature within ViewControllers
* Creation of multiple instances of the same views, each with their own ViewController and state
* Use of Promises
* Use of sequential and parallel Promise chains
* Use of Contexts to facilitate communication between ViewControllers


## Running the App

Drop the application into a local web server and load up the index.html page in a current browser that supports client storage. You can add new scenarios, add affected items to scenarios, and edit or delete affected items and scenarios. Multiple scenarios can be opened and edited at the same time.

The application was written with CoffeeScript (located in the /coffee folder), but all of the generated JavaScript is also included (in the /app folder). The Sencha CDN system is used to load the final release of ExtJS 4.2.

## TODO

Upgrade to ExtJS5: http://docs.sencha.com/extjs/5.0/whats_new/5.0/whats_new.html
Upgrade to DeftJS5: http://www.sencha.com/blog/upgrading-deft-js-to-work-with-ext-js-5
Add Log In: http://docs.sencha.com/extjs/5.1/tutorials/login_app.html
More about DeftJS: http://www.sencha.com/blog/deftjs-loosely-coupled-mvc-through-dependency-injection
About CoffeeScript: http://blog.ssokolow.com/archives/2011/05/07/a-python-programmers-first-impression-of-coffeescript/
