# Musify App

Step into the world of Musify, a state-of-the-art music platform crafted using ReactJs and Firebase. Through seamless integration with the Deezer music API, Musify offers an immersive music experience like no other. <br />
Beyond offering an extensive library of songs, Musify elevates your music exploration with its intuitive interface and a plethora of features designed to empower your musical journey.

## 📃 Table of Contents

- [Description](#-description)
- [Screenshots](#-screenshots)
- [Technologies](#-technologies)
- [Features](#-features)
- [Live demo](#-live-demo)
- [Launch](#-launch)
- [Misc](#-misc)
  - [Firebase Setup](#-firebase-setup)

## 📝 Description

Musify redefines the way you enjoy music by offering an enhanced listening experience. Featuring a sleek and user-friendly interface, users can effortlessly log in, explore, and indulge in their preferred tracks. Powered by ReactJs for dynamic frontend capabilities and Firebase for robust backend support, Musify ensures a seamless music journey.  
Experience uninterrupted music playback with Musify's array of features, including user authentication, intuitive song controls, comprehensive search options, playlist customization, and a personalized theme selector.  
The application was created in order to replace all analogues. Such as Spotify, which is no longer available in our country; SoundCloud, which does not have an excellent interface; YandexMusic, which does not always correctly display customizable collections, and frankly it is expensive.

## 📸 Screenshots

![Main screen](.github/screenshots/screenshot.png 'Main screen')

## 🛠️ Technologies

- `React`
- `Vite`
- `React Query`
- `Tailwind`
- `Firebase (Authentication, Firestore, Storage)`
- `Deezer Music API`

## 🦄 Features

- **User Authentication:** Sign in, sign up, and password reset functionalities.

- **Playback Controls:** Play, pause, skip, and loop songs with ease.

- **Volume Control:** Adjust volume, mute/unmute while enjoying your music.

- **Search Functionality:** Search for songs by song name, artist name, or album name.

- **Like Songs:** Like your favorite songs to build a personalized collection.

- **Playlist Creation:** Create and manage playlists tailored to your taste.

- **Song Details:** Explore song details, including cover image, singer, and album information.

- **Persistent Music Player:** A music player component accessible across all pages, allowing uninterrupted music playback.

- **Cross-Page Playback:** Keep the music playing while navigating through different sections of the app.

- **Theme Switcher:** Fully customizable theme switcher to personalize your visual experience.

## 🎥 Live demo

Check out the live demo of app [here](https://musify-app-1.vercel.app/)

## 🚀 Launch

To run the project in your local environment, follow these steps:

1. Clone the repository to your local machine.
2. Run `npm install` or `yarn` in the project directory to install the required dependencies.
3. Create a new .env file and add the necessary firebase configurations.

   ```
   VITE_PUBLIC_CORS_URL={your cors url}
   VITE_PUBLIC_AUTH_RESET_PASS_ACTION_URL={your auth reset pass action url}
   VITE_PUBLIC_DEEZER_API_URL={your deezer api url}
   VITE_PUBLIC_FIREBASE_STORAGE_BUCKET={your firebase storage bucket}
   VITE_PUBLIC_FIREBASE_PROJECT_ID={your firebase project id}
   VITE_PUBLIC_FIREBASE_AUTH_DOMAIN={your firebase auth domain}
   VITE_PUBLIC_FIREBASE_API_KEY={your firebase api key}

   ```

4. Run `npm run dev` or `yarn dev` to get the project started.
5. Open [http://localhost:5173](http://localhost:5173) (or the address shown in your console) in your web browser to view the app.

## 👾 Misc

### 🔥 Firebase Setup

1. Create a Firebase project here.
2. Obtain your Firebase configuration details.
3. Enable Authentication, Firestore, and Storage services.
4. Deploy the firestore security rules/indexes and storage security rules if you are on a paid plan OR copy and paste them if you are not on a paid plan.
5. Locate the above rules/indexes in the following files
   - firestore security rules - `firebase/config/firestore.rules`
   - firestore indexes - `firebase/config/firestore.indexes`
   - storage security rules - `firebase/config/storage.rules`
6. Customize password reset custom action URL from your firebase authentication dashboard. Go to Authentication, click on Templates menu, select Password reset tab and click on "Customize action URL" link. Add {domainURL}/verify-reset-password, eg - http://localhost:5173/verify-reset-password
