# Uber Ride

Create a single-page web application that visualizes the semantic model
described below, given its entities, attributes, and associated rules.
Render a demonstrative example of this semantic model and give
interactive means (a toolbar with buttons) to manipulate it according to
the actions and rules given.

## Application requirements

-   Make this project a simple single-page web application.
-   Use vanilla JavaScript.
-   The primary view should be a three.js rendered view that fills the
    browser window.

## Context

This model represents a typical Uber ride in an urban environment.

## Entities

The application should represent the following entities:

1.  riders
2.  drivers
3.  vehicles
4.  trips
5.  pickup locations
6.  destinations
7.  routes
8.  roads

## Entity Attributes

Describe each entity with the following parameters:

-   Rider
    -   location (point)
    -   destination (point)
-   Driver
    -   location (point)
    -   availability (boolean)
-   Vehicle
    -   location (point)
    -   capacity (number)
-   Trip
    -   status (text)
    -   estimated time (minutes)
    -   fare (number)
-   Pickup Location
    -   coordinates (point)
-   Destination
    -   coordinates (point)
-   Route
    -   path (polyline)
    -   distance (meters)
    -   estimated travel time (minutes)
-   Road
    -   path (polyline)
    -   traffic level (number)

## Relationships

-   a rider requests a trip
-   a driver accepts a trip
-   a driver operates one vehicle
-   a trip has one rider and one driver
-   a trip starts at a pickup location
-   a trip ends at a destination
-   a route connects the pickup location and destination
-   a route contains one or more roads
-   traffic conditions affect a route

## Actions

-   riders may request a trip
-   drivers may accept or reject a trip
-   riders may cancel a trip
-   drivers may start a trip
-   vehicles may move along a route
-   routes may be recalculated based on traffic conditions
-   trips may be completed when the vehicle reaches the destination
