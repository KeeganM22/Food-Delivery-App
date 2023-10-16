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

### Issue 
For the storage of data, we must decide whether we:
  - Store things remotely or locally
  - Encrypt or keep the data unencrypted

### Decision 
We will store sensetive data remotely and encrypted, while keeping local (non sensitive) data unencrypted. 


### Status

Refer to the section labled "Decision" . Open to re-evaluation as problems arise, and time constraints
## Details

### Assumptions

- Our team is capable of implementing two forms of storage and encryption
- That there are resources out there to help us learn about what we need to do
- That there are frameworks that allow us to do what we want

### Constraints

- We only have 8 weeks to develop this app. It may not be feasible to implement these security features.
- We lack the expertise to know if we have adequate data security measures.

### Positions

-We considered using unencrypted data for local and remote storage. We deemed that this would be incredibly reckless as we would be storing PII and payment information.

-We considered keeping all of the data local. This would run the risk of bad actors being able to easily attain PII and payment information. We opted not to do this. Furthermore, all data would be locally stored which would not be scalable as restraunts and reviews increased.

### Argument

Our solution mixes the best of both worlds, allowing 

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
