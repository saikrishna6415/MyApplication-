# Native App with React Native SDK Integration Guide

This README provides a guide for integrating a React Native app as a SDK into a native Android app.

## Overview

This is a native Android app that has integrated a React Native app as a SDK. React Native allows you to build mobile apps using only JavaScript. It uses the same design as React, letting you compose a rich mobile UI from declarative components. By integrating a React Native app as a SDK, you can leverage the power and ease of React Native development within your native Android app.

## Steps for Integration

1. **Add the React Native app as a SDK in your project**: You can do this by adding the following line in your `build.gradle` file.

2. **Implement the AAR in a Native Android Project**
   a. Import the AAR: Create a libs folder in android/app and copy your generated AAR file.
   b. Add React Native’s Maven Repository: Make sure your native Android project can access React Native dependencies by adding the repository in the build.gradle file.
   c. Include Necessary Dependencies: Add required dependencies in your app’s build.gradle.
   d. Modify the `MainApplication.java` file as per the provided example.
   e. Add `ReactNativeActivity` in `AndroidManifest.xml` file.

3. **Launching React Native Content**: To display React Native content within your Android app, initiate the `ReactNativeActivity`. For example, in your `MainActivity.java`, you can start the `ReactNativeActivity` using an `Intent`.
