---
title: EstimoteUnity
permalink: /docs/estimote_unity/
---

### Variables
* BeaconRegions
  * These are the beacon regions (UUID's) you want to scan for.
* ForegroundScanConfig
  * The scan period and wait time for foreground scanning.
* BackgroundScanConfig
  * The scan period and wait time for background scanning.
* EstimoteCloudAppId
  * Your Estimote App ID.
* EstimoteCloudAppToken
  * Your Estimote App Token.

### Events
* OnInitEstimoteComplete
  * An event called when the Estimote SDK has been setup.
* OnInitEstimoteCloudComplete
  * An event called when the Estimote Cloud SDK has been setup.
* OnStartedScanning
  * An event called when scanning has started.
* OnStoppedScanning
  * An event called when scanning has been stopped.
* OnDidRangeBeacons
  * An event called when beacons have been found, returning a list of EstimoteUnityBeacons.
* OnFetchedBeaconCloudDetailsSuccess
  * An event called we have have fetched the cloud details for a beacon.
* OnFetchedBeaconCloudDetailsError
  * An event called when we failed to get the cloud details for a beacon.

### Methods
* Initialize
  * This method must be called at the before you make any other calls. It will initiaise the core Estimote SDK and the Estimote Cloud SDK if you have it enabled.
* StartScanning
  * Calling this will start scanning for beacons. If any initialization needs to happen first it will automatically call this for you.
* StopScanning
  * Calling this will stop scanning for beacons. Once this has been called you will have to make a call to StartScanning() to receive more updates.
* GetBeaconCloudDetails
  * Calling this method will retrieve extra information about the beacon from Estimotes Cloud SDK. You can either pass in a UUID, Major and Minor values or an instance of an EstimoteUnityBeacon class.
