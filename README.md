# Mobile Development Environment Setup

## Objective
This document outlines the steps I took to set up my mobile development environment using Expo for React Native.

---

## My Setup Process

### 1 Installed Expo Go on Android
I first installed **Expo Go** on my Android device from the [Google Play Store](https://play.google.com/store/apps/details?id=host.exp.exponent).

---

### 2 Registered an Expo Account
After installing Expo Go, I registered an account within the app to enable testing and project management.

---

### 3 Setting Up Expo with React Native

To create a new Expo project, follow these steps:

#### 1. Install Node.js
Ensure you have **Node.js 16** or a **supported version (LTS recommended)** installed.  
Node.js **17+ and higher** may cause issues with `npm install -g expo-cli` and `npx create-expo-app@latest APP-NAME`.

You can check your Node.js version by running:

```sh
node -v
```

If you're on Node.js 17+ and encounter issues, consider downgrading to Node.js LTS (e.g., 16.x) using **nvm**:

```sh
nvm install 16
nvm use 16
```

#### 2. Install Expo CLI

If you're using **Node.js 16 or lower**, you can install Expo globally:

```sh
npm install -g expo-cli
```

However, if you're on **Node.js 17+**, avoid installing `expo-cli` globally. Instead, use `npx create-expo-app@latest APP-NAME`
`

---

### **Create Your First Mobile App**

#### Steps
1. Navigate to your project directory:
   ```sh
   cd prodev-mobile-setup
   ```
2. Initialize a new Expo project:
   ```sh
   npx create-expo-app@latest .
   ```
3. Modify the home screen:
   - Open `app/(tabs)/index.tsx`.
   - Change **Welcome!** to **First App Created**.
4. Run and test your application:
   ```sh
   npx expo start
   ```
5. Reset the application:
   ```sh
   npm run reset-project
   ```

---

## Resetting the Project
If you encounter issues with dependencies, caching, or unexpected behavior, you can reset the project using:

```sh
npm run reset-project
```

### Effect of `npm run reset-project`
Running this command will:
1. **Remove `node_modules` and `package-lock.json`** – Ensures dependencies are reinstalled from scratch.
2. **Clear Metro Bundler Cache** – Removes outdated JavaScript bundles.
3. **Clear Watchman Cache** – Resets file watchers.
4. **Reinstall Dependencies** – Runs `npm install` to fetch fresh packages.
5. **Reset Expo Cache** – Ensures a clean build environment.

If issues persist, you can manually reset the project with:

```sh
rm -rf node_modules package-lock.json
npm install
expo r -c
```

---


## Repository Information
- **GitHub Repository**: `prodev-mobile-setup`

---

## Author
**Florence Kamau**
