# J-MUSIC

A responsive, single-page music discovery website.

The public Admin preview is available at `admin.html`. It contains sample dashboard data and front-end-only review actions; it is not a secure or connected admin system.

## Run locally

Open `index.html` in a browser. The music player uses demo audio. User sign-up and login use Firebase Authentication after the project is configured; artist forms are still a UI demonstration.

## Configure user sign-up with Firebase

1. Create a Firebase project in the [Firebase Console](https://console.firebase.google.com/).
2. Add a **Web app** to the project, then copy its web configuration values into `firebase-config.js`.
3. In **Authentication → Sign-in method**, enable **Email/Password**.
4. In **Authentication → Settings → Authorized domains**, add `onuja070-lang.github.io`.
5. In **Authentication → Templates**, configure the email verification message and sender settings.

Users create their own accounts with a username, email, and password, then confirm their email before logging in. The username is saved as the Firebase Auth display name; usernames are not guaranteed unique until a database with appropriate security rules is added. Firebase web-app configuration is intended for public client use; protect backend data separately with Firebase Security Rules. **Never put service-account credentials or private keys in this website or its public repository.**

## Publish with GitHub Pages

1. Push the contents of this folder to the `main` branch of `onuja070-lang/J-MUSI`.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/(root)`, then save.
4. After GitHub Pages finishes deploying, the site will be at `https://onuja070-lang.github.io/J-MUSI/`. The dashboard preview is at `https://onuja070-lang.github.io/J-MUSI/admin.html`.
