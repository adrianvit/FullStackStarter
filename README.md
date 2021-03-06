# FullStackStarter
A starter kit to allow combining various backend and frontend starter projects doing very basic operations

Requirements: NodeJs latest (6.7 at the time this was built)
MongoDB : external requirement

* <b>NodeJS</b>
   A very basic nodeJS server which connects to a mongoDB
   - Setup steps:
      * cd NodeJS
      * npm install
      * node bin/www
   - Provided functionality
      * access on port 4000
      * provides two api endpoints:
         * GET /api/users : provides back an array of users from the mongo collection
         * GET /api/profile : provides the profile information for the currently authenticated user
         * POST /api/signup : creates a new user in the mongo collection
         * POST /api/login : authenticates a user

* <b>ReactClient</b>
   - A very basic react client build with
      * material UI library for UI elements
      * redux for managing the React flow
   - Setup steps
      * cd NodeJS
      * npm install
   - Build (this will create the packaged app in the dist folder within the app):
      * npm run build
   - Develop
      * npm start (this will start a webpack bundler which repackages the app while it's being developed - app is served from port 3000)
      
* <b>ReactNative</b>
   A very basic react native client
   - Required dependencies:
      * Android Studio 2.0
      * SDK Tools 25.0.10 or higher
      * Android emulator
      * follow instalation steps provided at: https://facebook.github.io/react-native/docs/getting-started.html (remember to choose your OS and your platform - we will focus on Android as platform)
      * install the Android SDK's compatible with your phone
   - Setup steps
      * cd ReactNative
      * npm install -g react-native-cli (use sudo in case of MacOS)
   - Running
      * react-native run-ios
      * react-native run-android
