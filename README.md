I built this app by following the [Ionic Guide](ionicframework.com/docs/guide) This document is for future reference.

Ionic is a framework for web developers to build native apps with html, css, and javascript.  It's built with Angular, but you can use another mvc, although if you write with React, you'll probably write with React Native.

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
