# Intelligent Crowd Management System for COVID-19 

### Introduction

The idea of this project is to develop an intelligent crowd management system that will let a user know whether if it's safe to go to a superstore or restaurant of their choice and using the place safety grade presented, they can delay their shopping time and plan to go at a time when there is less crowd and it also recommends the user different superstores or restaurant with place safety grade, within a certain distance as set by the user. The system will also recommend nearby superstores/restaurants sorted with respect to place safety grade and its open-close status. This application will also help the stores and restaurants  to get control over the crowd management so that it puts less strain on their store workers and supply chain demands in these difficult times. The application tells a user who is looking to go out for grocery shopping or eating at a restaurant, about the current place safety grade which we have divided into 3 grades namely “Very safe”, “Safe” and “Hard to maintain social distancing”.

### Technologies relevant to this project

We have used Google cloud platform for the cloud service needed for hosting our application. Our application is divided into web tier and app tier and the web tier interacts with app tier through the generated url link. Both the web tier and app tier are hosted on Google app engine. We have used MongoDB atlas for storing the data. We have also used multiple google APIs for getting the relevant data. For coding this application we have flask, which is a micro web framework for python.

### System Architecture and Design on GCP

#### Application Cloud Architecture

![System on Google cloud](./Images/OverviewDiagram.png)

#### Live System Architecture

![Live System on Google cloud](./Images/LiveUpdatesAppTier.png)

#### Analytics System Architecture

![Live System on Google cloud](./Images/AnalyticsAppTier.png)

### Quick example of system

In the following example, we have checked the Restaurant Live Status for the cheesecake factory, in Chandler, AZ and selected the range of 1 mile for recommendation of other restaurants. We found that Live status and expected future status of the desired location is correctly labelled and properly pinned in the map. Also, the recommended locations are correctly ranked based on the Safeness and the opening status of the restaurant.

![Example of LiveUpdates of queried Restaurant](./Images/QueriedDestination.png)

In the map we have used the following markers to help the user to identify the status of safeness of the location the user wants to visit and the recommended locations. Following are the importance of the each colored marker in the map:
1. ![Green Marker](./Images/greenMarker.png)Represents a very safe place to visit.
2. ![Yellow Marker](./Images/yellowMarker.png)Represents a safe place to visit.
3. ![Red Marker](http://www.google.com/mapfiles/marker.png) Represents unsafe and hard to maintain social distancing.
4. ![Green Arrow](http://maps.google.com/mapfiles/arrow.png) Represents the location which user has selected to visit.

![LiveUpdates of queried Restaurant and recommendation](./Images/LiveUpdateOfDestination.png)




