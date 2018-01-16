---
title: EstimoteUnityBeacon
permalink: /docs/estimote_unity_beacon/
---
This class represents a beacon returned from the Estimote SDK. It contains all of the core information relating to a beacon. Although this is named "EstimoteUnityBeacon" this is the same type returned for any iBeacon being ranged.

### Variables
* UUID
  * This is the proximity UUID for this beacon
* Major
  * This is the beacons major ID
* Minor
  * This is the beacons minor ID
* BeaconRange
  * This is a high level representation of the beacons distance from the device
* RSSI
  * This is the signal strength if the beacon, measured in decibels
* Accuracy
  * The accuracy of the proximity value, measured in meters from the beacon
* LastSeen
  * When the beacon was last seen by the device
