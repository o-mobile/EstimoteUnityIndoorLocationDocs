---
title: EstimoteUnityBeaconCloudInfo
permalink: /docs/estimote_unity_beacon_cloud_info/
---

This class houses details returned from the Estimote Cloud SDK. When fetching the cloud details for a beacon an instance of this is returned. Some of the details can be configured online using the Estimote Cloud Portal. This class is specific to Estimote beacons only.

### Variables
* UUID
  * This is the proximity UUID for this beacon
* Major
  * This is the beacons major ID
* Minor
  * This is the beacons minor ID
* BeaconName
  * This is the name that has been assigned to the beacon through the Estimote Cloud Portal
* Color
  * This is the color of the beacon in string form
* BatteryLifeDays
  * This is how long the beacons battery will last, measured in days
* MacAddress
  * This is the beacons mac address
