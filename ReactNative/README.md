Core Components of React Native:
1. **View**: The `View` component is similar to a `div` in web development. It is used to create a container for other components, helping with layout and styling. It's a fundamental building block for creating the user interface in React Native.

2. **Text**: The `Text` component is used to display text on the screen. It can be styled, formatted, and used to render text-based content to the user.

3. **Image**: The `Image` component is used to display images, just like the `img` tag in web development. It allows you to show images from various sources, such as local files or network URLs, and provides options for resizing and styling.

React Native solves the problem of creating mobile apps that look and feel native to the platform (iOS and Android) while using a single codebase. It is called "native" because it allows developers to build mobile applications using JavaScript and React, but the final output is a native app that can access device features and provide a user experience consistent with the platform's native apps.

Building Blocks of a React Native app compared to a React app:
- React Native apps use native components like `View`, `Text`, and `Image` to render the user interface, whereas React apps use web-based components like `div`, `span`, and `img`.
- In React Native, styling is done using a subset of CSS that is compatible with mobile platforms, while in React, traditional CSS is used.
- React Native apps can use platform-specific code to access device features, while React apps are primarily designed for web browsers and don't have direct access to native features.

Expo:
Expo provides a development platform and set of tools to simplify the process of building React Native applications. It aims to manage much of the complexity of app development.

Expo's solution:
- Expo provides a managed workflow for React Native development, which means it handles many aspects of the development process, such as building, testing, and deploying your app without requiring you to configure native code or tools.

Difference between React Native and Expo:
- React Native is the core framework for building mobile apps using JavaScript and React. It provides more flexibility but requires manual configuration for some native features.
- Expo is a set of tools and services built on top of React Native. It offers a managed workflow, simplifying development but with some limitations. You might not have access to certain native modules and libraries in Expo.

Expo Snack:
Expo Snack is an online tool provided by Expo that allows developers to write and run React Native code directly in their web browser. It's a convenient way to prototype, share, and test React Native components and apps without setting up a local development environment.

Ejecting in the context of Expo:
"Ejecting" in the context of Expo means transitioning from Expo's managed workflow to the standard React Native development environment. When you eject from Expo, you gain more control over your project's configuration, including access to native code and dependencies that Expo abstracted away.

When not to eject:
You should not eject from Expo if you want to continue using Expo's managed workflow and prefer the simplicity it offers. Ejecting is an irreversible action, and if you're comfortable with Expo handling most of the complexities, there may be no need to eject.

Why you might choose to eject:
You might choose to eject from Expo when you require more advanced customizations, need to include specific native modules or libraries not supported by Expo, or want greater control over your project's dependencies and configuration. Ejecting allows you to take your Expo project to the standard React Native development environment, offering more flexibility but also more responsibility for managing your app's configuration and dependencies.