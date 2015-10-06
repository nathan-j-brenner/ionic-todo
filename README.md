I built this app by following the [Ionic Guide](ionicframework.com/docs/guide) This document is for future reference.

Ionic is a framework for web developers to build native apps with html, css, and javascript.  It's built with Angular, but you can use another mvc, although if you write with React, you'll probably write with React Native. "It's built with Angular" just means that Ionic has built in custom Angular directives.

##Installing your app
1. Create application directory: `ionic create ionic-todo blank`
2. Add native platforms: Since I'm working on a mac, I already have the ios platform.
 `ionic platform add android`
3. build and emulate: `ionic build ios` `ionic emulate ios`
	If ionic emulate ios fails, `npm install -g ios-sim`
	ios Simulator should open in a separate window
##Starting your app
4. View `www/index.html`. ngAnimate and ngSanitize comes with `ionic.bundle.js`
5. Create the side menus: One will contain the menu content, the other will be on the left side by applying the attribute `side="left"`
6. Add header content to each menu
##Testing your app
7. Desktop browser testing: `ionic serve`
This opens your app in a browser.  As you make changes to the app with the server running, the changes will show in the browser.  Also, since you created a left content area, right click on mouse and swipe right to see the area.  If you click again, the area goes away
8. Simulator testing: `ionic build ios` `ionic emulate ios`.  You can do the same with android, but it didn't work on my mac.
9. Native app testing: if on mac, you have to register with Apple Developer and pay $99 per year so I won't be doing this unless it's critical
##Building the app
To learn more on angular, visit [egghead.io]() and [thinkster.io]()
10. Add content in the main menu with ng-repeat.  Create a controller with an array of tasks in `$scope.tasks`.
11. Create Tasks:  Create a script tag with the type `text/ng-template` and add a div.modal with header that says `New Task` and a cancel button, with a ng-click directive that initiates `closeNewTask()`. Create a form that has a single input so on submit the value get's pushed into the scope tasks array.  Add a button in the main menu header to trigger the modal to open.
12. In app.js: add in `$ionicModal` as a dependency in the controller, and create the methods for creating/loading in the modal and submitting a form
13. Add projects
...Add more about the last step concerning the changes in app.js

