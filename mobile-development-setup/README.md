# Mobile Development Environment Setup

## Objective
This document outlines the steps I took to set up my mobile development environment using Expo for React Native.

---

## My Setup Process

### 1️⃣ Installed Expo Go on Android
I first installed **Expo Go** on my Android device from the [Google Play Store](https://play.google.com/store/apps/details?id=host.exp.exponent).

### 2️⃣ Registered an Expo Account
After installing Expo Go, I registered an account within the app to enable testing and project management.

### 3️⃣ Attempted to Install Expo CLI
I tried installing **Expo CLI** globally using:
```sh
npm install -g expo-cli
```
However, I encountered an issue due to an outdated version of **Node.js**.

### 4️⃣ Upgraded Node.js to Version 20
To resolve the issue, I upgraded to the latest **Node.js LTS (version 20)** by downloading it from the [official Node.js website](https://nodejs.org/). After upgrading, I verified the installation:
```sh
node -v
npm -v
```

### 5️⃣ Successfully Installed Expo CLI
After upgrading Node.js, I was able to install Expo CLI successfully:
```sh
npm install -g expo-cli
```

### 6️⃣ Verified the Installation
I confirmed that Expo CLI was installed correctly by checking its version:
```sh
expo --version
```

---

## Challenges Faced
- Initially had an **older version of Node.js**, which caused issues when installing Expo CLI. This was resolved by upgrading to **Node.js 20**.

---

## Repository Information
- **GitHub Repository**: `prodev-mobile-setup`
- **Directory**: `mobile-development-setup`
- **File**: `README.md`

---

## Author
**Florence Kamau**

