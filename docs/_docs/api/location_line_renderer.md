---
title: LocationLineRenderer
permalink: /docs/location_line_renderer/
---

A location renderer using the Unity LineRenderer component.

### Variables
* WallLine (LineRenderer)
  * The line renderer used to draw the walls.
* Player (Transform)
  * The players transform.
* PlayerLerpSpeed (float)
  * The smoothing value for the players position.
* ShowBeacons (bool)
  * Whether to render beacons or not.
* BeaconScale (Vector3)
  * The scale at which to render the beacons.

### Methods
* SetLocation (Location location)
  * Sets the Location property for this location renderer.
* UpdatePlayerPosition (LocationPosition position)
  * Called when a players position has been updated.
