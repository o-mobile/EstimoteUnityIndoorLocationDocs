---
title: IndoorLocation
permalink: /docs/indoor_location/
---

This class is the core of the Indoor Location plugin. Its handles the communication with the Estimote Indoor Location SDK to retrieve locations and start/stop positioning within a location.

### Variables
* EstimoteCloudAppId (string)
  * Your Estimote App ID
* EstimoteCloudAppToken (string)
  * Your Estimote App Token
* ProvideOrientation (bool)
  * Whether the IndoorLocation SDK (iOS only) will provide orientation information for the user
* IndoorLocationManagerMode (IOSIndoorLocationManagerMode)
  *  The mode for the Indoor Location manager which effects how position updates are delivered (iOS only)
* LocationRenderer (BaseLocationRenderer)
  * The renderer to be used for the locations
* AutoSetLocationOnRenderer (bool)
  * If true the location will automatically be set onto the Location Renderer assigned
* EnableEditorLocationSuccessCallback (bool)
  * Whether to enable rendering of debug JSON locations within the editor
* DebugLocationJSON (string)
  * Debug JSON that can be used within the editor to test location rendering

### Events
* OnInitIndoorLocationSuccess
  * An event called when the SDK has been initialized
* OnPermissionsChecked
  * An event called when permissions have been checked
* OnRetrieveAllLocationsSuccess
  * An event called when all locations have been retrieved successfully
* OnRetrieveAllLocationsFailure
  * An event called when all locations were failed to be retrieved
* OnRetrieveLocationSuccess
  * An event called when a specific location has been retrieved successfully
* OnRetrieveLocationFailure
  * An event called when a specific location has failed to be received
* OnStartPositioningFailed
  * An event called when positioning failed to start
* OnStartPositioning
  * An event called when positioning has started
* OnStopPositioning
  * An event called when positioning has stopped
* OnPositionUpdate
  * An event called for position updates
* OnPositionOutsideLocation
  * An event called when the user is outside the location

### Methods
* Initialize
  * This method must be called at the before you make any other calls. It will initialize the core Indoor Location SDK.
* RequestPermissions
  * This will request the necessary permissions to use the Indoor Location SDK. Android only.
* GetAllCloudLocations
  * This will request all of the locations within your account.
* GetCloudLocation (string indoorLocationId)
  * This will request a location by its identifier.
* StartPositioning
  * This will request position updates to be started.
* StopPositioning
  * This will request position updates to be stopped.
