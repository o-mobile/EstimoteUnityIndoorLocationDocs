---
title: Location
permalink: /docs/location/
---

This class represents a Location from the Estimote Indoor Location SDK.

### Variables
* LocationName (string)
  * The name of the location
* IsPublic (bool)
  * Whether the location is public or not
* Owner (string)
  * The email of the owner of this location
* Orientation (double)
  * The orientation of this location
* Walls (List<LocationWall>)
  * A list of walls within this location
* Beacons (List<LocationBeacon>)
  * A list of beacons within this location

### Methods
* GetMaxX
  * Gets the maximum X value from all walls.
* GetMinX
  * Gets the minimum X value from all walls.
* GetMaxY
  * Gets the maximum Y value from all walls.
* GetMinY
  * Gets the minimum Y value from all walls.
