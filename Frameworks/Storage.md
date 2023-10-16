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

Our solution mixes the best of both worlds, allowing for less calls for non-sensitive information and protection for PII and payment information. It also reduces the amount of storage needed locally as it will only be used to store nescessary data. Sensitive data will be encrypted locally.

### Implications

-More time will need to be dedicated to implementing this properly.
-We may not be able to implement these features properly.
-Potential problems may come from our lack of experience in storage, encryption, and safe data storage practices.
-We will have to do a ton on research about data storage best practices, and how well it meshes with our tech stack.

## Related

### Related decisions:

This choice may heavily impact how much time we can allocate to other (potentiall more critical) aspects of the project. It will also affect how we implement data storage with Mongo DB, in addition to potentially conflicting with our tech stack.

### Related requirements:
-Need solid data protection measures
-Need a definitive answer on where data will be stored
### Related artifacts:
-Will affect all codebases, components, and modules developed for the app.
### Related principles:
-Application security
-Data security
-Ease of development
-Data storage

## Notes
This will greatly increase our understanding of data protection and how databases work in the wild.
