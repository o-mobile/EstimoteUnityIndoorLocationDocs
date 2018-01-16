---
title: Quick Start Guide
permalink: /docs/quick_start_guide/
---
There are a few quick and easy steps to get started with the plugin. Follow the instructions below to get started.

1. Use the menu command (Window/O-Mobile/Indoor Location/Instantiate Indoor Location Objects) to add the required GameObjects and scripts to your scene.
2. You now have two new GameObjects in your scene. These are the core scripts which are required to run Estimote Unity Indoor Location.
3. Select the IndoorLocation GameObject and inside the inspector open the General tab.
4. Enter your Estimote AppID and AppToken in the respective fields. If you need to create new ones use the button to do so.
5. Create a new GameObject and add the IndoorLocationDemoController to it.
6. Assign the IndoorLocation variable on the IndoorLocationDemoController and ensure you have entered a location ID you want to use.
7. Ensure there are no warnings on the IndoorLocation inspector. If there are then follow the setup process (by clicking the button within the warnings panel).
8. Complete! You are now able to build to your chosen platform and start testing.
9. When building to a device please ensure you have targeted the correct OS/API levels as stated under the System Requirements section above.
