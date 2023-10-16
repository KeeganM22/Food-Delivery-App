# Food-Delivery-App
App developed in Mobile Application class. A food delivery app


# Assignment Architectural Decisions 

 - [Summary](#summary)
  - [Issue](#issue)
  - [Decision](#decision)
  - [Status](#status)
- [Details](#details)
  - [Assumptions](#assumptions)
  - [Constraints](#constraints)
  - [Positions](#positions)
  - [Argument](#argument)
  - [Implications](#implications)
- [Related](#related)
  - [Related decisions](#related-decisions)
  - [Related requirements](#related-requirements)
  - [Related artifacts](#related-artifacts)
  - [Related principles](#related-principles)
- [Notes](#notes)

## Summary

Choosing a mobile app development framework that provides a native feel, rapid development, and cross-platform support.

### Issue 
For the mobile app, we require a development framework that:

-Allows rapid development and deployment for Android.
-Provides a native look and feel.
-Supports integration with external libraries and services, like MongoDB.

### Decision 
Opted for React Native.


### Status

Decided on React Native. Open to re-evaluation as new frameworks or major updates to existing ones emerge.

## Details

### Assumptions

-We are targeting both Android (as per project requirement) and possibly iOS in the future.
-The team is familiar or can quickly adapt to JavaScript-based development.
-Integration with other services (like MongoDB) is feasible and well-supported.

### Constraints

-The chosen framework should not require learning an entirely new language or paradigm.
-Must have a robust community and support for troubleshooting and library/plugin availability.

### Positions

-Native Development (Java/Kotlin for Android): While it offers the most control and performance, it requires platform-specific development, increasing time and resources.
-Ionic: Uses web technologies and gives a more web-app-like feel. Might not provide the full native experience we desire.
-Cordova: Similar to Ionic but might feel more like a web app than a truly native app.
-Framework7: Has a native feel, but community support and available libraries might be limited compared to React Native.
-Native Script: Provides direct access to native APIs but may have a steeper learning curve compared to React Native.
We opted for React Native given its widespread adoption, vast community support, and the ability to create truly native apps using JavaScript.

### Argument

React Native emerges as a favorable choice given its capability to produce apps with native performance, its extensive community support, and its compatibility with popular databases and services. Additionally, the use of JavaScript makes it more approachable for developers familiar with web development.

### Implications

-Faster time-to-market due to cross-platform development.
-A wide range of libraries and plugins available.
-Potential challenges may arise when needing very platform-specific features or optimizations, though React Native's capability to integrate native modules can address this.

## Related

### Related decisions:

The choice of React Native can influence the libraries and plugins we opt for in later stages, especially for UI components and state management.

### Related requirements:
-Need for a native-feel app.
-Desire for quick development and prototyping.
### Related artifacts:
-Will affect all codebases, components, and modules developed for the app.
### Related principles:
-Prioritize user experience.
-Efficiency in development.

## Notes
React Native offers the "Learn once, write anywhere" principle, which can be beneficial for future expansions or platforms.
