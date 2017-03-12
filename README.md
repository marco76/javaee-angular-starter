#Angular CLI, Java EE and REST : tutorial and quick starter code for Hello World
Problem: we need  a new web application that uses Java EE as backend and Angular as frontend. It should be easy to configure.

The scope of the application is limited (1 angular route, 1 http service, only a JSON ressource), this allow you to have a pretty clean app.
I will build another app to shows some features.

#####Features
- frontend built and compatible with [Angular CLI]
- configured to use the development and production mode of WebPack
- ready to use out of the box
- build a WAR file compatible with Java EE servers (JBoss, Payara/Glassfish etc.)
- it comes with all the nice features of Angular CLI: tests, good practices etc.

###How to install
##### Prerequisites
-you need maven, npm, git and an application server Java EE

##### Production mode
1. clone the git project
2. from the root of the project launch `mvn package` this generates a package named _ROOT.war_ in the _PROJECT/server/target_ directory
3. you can deploy this package in your favourite application server. The Angular application should answer at the requests to _http://localhost:8080_

##### Development mode
1. clone the git project
2. You can start the server using your favourite IDE. The project uses a standard Maven directory structure. You need to configure the server to deploy the _server.war_ artifact.
2. from the _PROJECT/client/src_ directory install the npm packages : `npm install`
3. launch the client with `ng serve`. The client uses the port 4200 (default for Angular CLI) and you can navigate to _http://localhost:4200_

### The result
(img)
The result is not particularly fancy. It show the result of a call to a Java REST service ... but hey, you have a ready to go configuration based on Java EE and Angular that follows the Angular best practices.
