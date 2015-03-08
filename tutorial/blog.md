# Location Tracker Part 3: Add a middle tier to manage users, with Node.js

In [Part 1](https://github.com/cloudant-labs/location-tracker-couchapp/blob/master/tutorial/tutorial.adoc) of this tutorial series we learned why location is so important to modern mobile apps and how to build the basic functionality. In [Part 2](https://github.com/cloudant-labs/location-tracker-angular/blob/master/tutorial/tutorial.adoc), we took that code and transformed it into a serious app using AngularJS. In both Parts 1 and 2, the Location Tracker application was built as a [CouchApp](http://docs.couchdb.org/en/latest/couchapp/). The cool thing about a CouchApp is that it can be hosted completely within Cloudant. This makes CouchApps great for demo applications like the Location Tracker. As an added bonus, you can quickly fork a CouchApp by replicating it into your own Cloudant account and have a fully-functioning application up-and-running in under 60 seconds. However, there are limitations to CouchApps.

Without a [middle tier](http://en.wikipedia.org/wiki/Multitier_architecture), building certain functionality becomes a challenge. The typical three-tier architecture includes a data tier, an application (or logic) tier, and a presentation tier. CouchApps eschew the traditional application tier and just include a data tier (Cloudant or CouchDB) and a presentation tier (HTML5, CSS and JavaScript). While possible to build _some_ application logic within Cloudant, there are practical limitations. This is because Cloudant is primarily intended to be used as a data layer.

[![Overview of a three-tier application including presentation tier, logic tier, and data tier](http://upload.wikimedia.org/wikipedia/commons/5/51/Overview_of_a_three-tier_application_vectorVersion.svg "Overview of a Three-Tier Application")](http://en.wikipedia.org/wiki/Multitier_architecture)

Let's take managing user access, for example. How would you go about building a user management system without an application tier? If you can figure out how to do this, I'd love to know! In [Part 3](tutorial.md) of this tutorial we build a Node.js application that handles user registration, login and logout. Additionally, we make the Location Tracker application deployable to [IBM Bluemix](https://console.ng.bluemix.net/) and update the map to display individual user locations, rather than one big map of all user locations.

[![IBM Bluemix logo](http://upload.wikimedia.org/wikipedia/commons/c/c7/IBM_Bluemix_logo.svg "IBM Bluemix")](https://console.ng.bluemix.net/)

⇒ **[Location Tracker Tutorial: Part 3](tutorial.md)**