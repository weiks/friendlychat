# Important lessons for working with c9.io

1) you cannot use localhost, so you have to use this command
2) you must grant auth access to your c9.io page

Altogether, here's what you need to do to get started

1) G: Fork the project on Github https://github.com/firebase/friendlychat
2) C9: create a nodejs space on c9.io based on that fork
3) F: Create a project in Firebase (console.firebase.google.com)
4) F: Copy the credentials from the project. You must click 2x in the console because of a bug.
5) F-C9: Paste the credentials in to web/index.html
6) run these commands in your c9 space (the second command solves the broken auth URL issue):
npm -g install firebase-tools
firebase login --no-localhost
firebase use --add
7) F: enable Google Auth (Auth > Sign in method)
8) F: OAuth redirect domains: add the C9.io domain.  This fixes the pop up disappearing
9) deploy to firebase hosting if you wish (must be in the correct directory):
cd web
firebase deploy
10) F: you can point a custom domain in the hosting panel

# Firebase Codelab: FriendlyChat

This is the source code for the Firebase FriendlyChat codelab. It includes start and end versions of the
code for Web, Android, Objective-C and Swift. To get started open the codelab instructions:

 - [Web Codelab](https://codelabs.developers.google.com/codelabs/firebase-web/).
 - [Android Codelab](https://codelabs.developers.google.com/codelabs/firebase-android/).
 - [Swift Codelab](https://codelabs.developers.google.com/codelabs/firebase-ios-swift/).
 - [Objective-C Codelab](https://codelabs.developers.google.com/codelabs/firebase-ios-objc/).


## How to make contributions?
Please read and follow the steps in the [CONTRIBUTING.md](CONTRIBUTING.md)


## License
See [LICENSE](LICENSE)
