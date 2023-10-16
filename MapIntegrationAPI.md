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

Choosing a map service API for location-based features in our mobile application

### Issue 
The mobile app requires location-based services like:

- Displaying restaurants or food outlets on a map.
- Providing delivery route visualization.
- Offering location-based search and recommendations.

### Decision 
Opted for Google Maps API.


### Status

Decided on Google Maps API. Will re-evaluate if project requirements change or new mapping solutions emerge that offer superior features.

## Details

### Assumptions

- Users are familiar with Google Maps and will find it intuitive.
- We will have access to reliable internet connectivity for fetching map data.
- The API will be primarily used for Android, as per project specifications.
- Android devices have the harware capabilities to support the Google Maps API.

### Constraints

- Google Maps API has associated costs after a certain number of requests.
- Reliable internet connection is necessary for real-time map functionalities.

### Positions

- OpenStreetMap: A free alternative, but might lack some of the advanced features or the polished UI of Google Maps.
- Mapbox: Offers robust features but has its own pricing and might require additional setup and learning.
- Here: Another alternative with extensive features but might have limitations in certain regions compared to Google Maps.
- After considering these options, Google Maps API was selected due to its widespread recognition, ease of integration, and comprehensive features.


### Argument

Google Maps is a globally recognized platform with detailed maps of most regions. The API provides a myriad of features, such as place search, route planning, and geolocation. The vast amount of documentation, tutorials, and community support makes integration and troubleshooting easier.

### Implications

- There will be a dependency on Google's infrastructure.
- The cost associated with the API will become a factor if the app scales with a significant user base.
- User trust may be higher given the familiarity with the Google Maps platform.

## Related

### Related decisions:

The choice of Google Maps API may affect other location-based services or integrations we might consider in the future.

### Related requirements:
- Reliable map data for user navigation and location services.
### Related artifacts:
- Will affect all app sections that utilize map or location-based features.
### Related principles:
- Prioritize user experience and familiarity.
- Scalability and reliability.

## Notes
While Google Maps is a preferred choice now, always be aware of the usage limits and potential costs. Monitoring and optimization will be crucial as the app gains more users.
