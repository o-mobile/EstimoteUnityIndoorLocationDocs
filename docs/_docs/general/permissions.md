---
title: Permissions
permalink: /docs/permissions/
---
Indoor Location requires some permissions to be granted on both Android and iOS.

### iOS
On iOS these are requested automatically by the system.

### Android
On Android they are not requested automatically if they are not present in your manifest. The permissions you require are:
* android.permission.BLUETOOTH
* android.permission.ACCESS_COARSE_LOCATION

There is a helper method within the Unity IndoorLocation class which lets you check if the required permissions have been granted or not. Currently we are unable to request these permissions for you but we are working on finding a solution for this.
