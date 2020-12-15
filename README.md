# Test app for deployment on Firebase

## How to deploy a React project on Firebase

### React

1. Run `npx create-react-app` to create a new React project.

2. Run `npm run build` to initially create the build directory.

### Firebase

3. Install the Firebase CLI by running `npm install -g firebase-tools` and then `firebase login`.

4. In a browser, log in to the Firebase website, use the Firebase console to create a new project, if you do not already have one to add this app to.

5. Configure this project as a Firebase app by running `firebase init` and clicking through the options. Some options of note are:

   - Type `build` when asked for public directory (not the default `public`)
   - Select `No` when asked to overwrite the already existing build/index.html file

6. In a browser, on the Firebase website, use the Firebase console to add this app to a project. Copy and paste the code it tells you to, eg `"site": "orangefrog",` into the firebase.json file.

7. To finally deploy, run `firebase deploy` or `firebase deploy --only hosting`.

The project should now be viewable via the hosted Firebase url, provided you have followed these steps in this order.
