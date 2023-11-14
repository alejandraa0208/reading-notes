# Class 41 Notes

## Reading

### getting started with react native

Name three Core Components of React Native and describe what they do.

View: The View component is a container that supports layout with flexbox, style, some touch handling, and accessibility controls. It maps directly to the native view equivalent on whatever platform the app is running on, like a UIView in iOS or an android.view in Android. It's similar to a div in HTML and is used to build other components.

Text: The Text component is used to display text. It supports styling through the style prop and is used for any kind of text rendering. In React Native, text must be rendered within a Text component (unlike in the web where text can be directly inside a div).

Image: The Image component is used to display images in the app. It can load images from various sources (like a local asset or a remote URL), and it supports a range of image manipulation capabilities.

What problem does React Native solve (why call it native)?

React Native primarily solves the problem of needing to write separate codebases for mobile platforms (iOS and Android). By using React Native, developers can write their app's logic in JavaScript and render it with native components, leading to native-like performance and look-and-feel on both iOS and Android from a single codebase. This significantly reduces development time and effort.

What are the building blocks of a React Native app? How does that compare to a React app?

React Native apps are built using native components like View, Text, and Image, instead of web components like div, span, and img. The logic is written in JavaScript, similar to React apps, but the rendering layer is native, which provides the performance and user experience of a native app.

### expo

What solution does expo provide?

Expo is a framework and platform for universal React applications. It provides a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.

Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the managed workflow.

What is the difference between React Native and Expo?

React Native is an open-source framework for building native apps using React. Expo, on the other hand, is a set of tools and services built on top of React Native. While React Native requires you to set up your development environment and manage native code, Expo provides a managed environment where much of this complexity is handled for you, especially beneficial for beginners or those who want to quickly prototype.

### expo snack

Checkout this tool. What does snack allow you to do?

Expo Snack is an online platform that allows you to write, run, and share React Native code in the browser. It's like a CodePen or JSFiddle for React Native, enabling quick prototyping and sharing of React Native applications without needing any local setup.

### ejecting

What does “eject” mean within the context of Expo?

"Ejecting" in the context of Expo means taking your Expo project out of the managed workflow and into the bare workflow, where you have full control over the native code (iOS and Android). This process generates the native project files you would need to continue working on your app outside of the managed Expo environment.

When should you not eject?

You don't need to add custom native modules that aren't supported by Expo.

You prefer to have Expo manage the complexities of the native build environment.

You are still in the experimental or prototyping phase of your project.

Why might you choose to eject?

You need to include custom native code or third-party native modules that are not supported in the Expo managed workflow.

You require more control over the native side of your project.

You are ready to move to a more traditional React Native development workflow for more flexibility.
