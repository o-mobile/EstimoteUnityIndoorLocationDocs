---
title: FAQ
permalink: /docs/faq/
---

### Does the plugin require any permissions on iOS/Android?
Yes, the plugin does require some permissions on iOS and Android. These are explained in the [permissions]({{ "/docs/permissions/" | prepend: site.baseurl }}) section in the documentation.

### When I build the APK from Unity there are errors?
On Android you cannot build the APK directly from within Unity. Instead you need to use the gradle build system to build an Android Studio project, which you can then load and build your application. The reason for these added steps is because the Estimote Indoor Location SDK requires various libraries that are synced using the gradle build system, and can only be done so using an Android Studio project.

### When I load the Android Studio project I get errors relating to gradle?
Please ensure you have completed the setup process within Unity (check the Quick Start Guide). This will copy the required files inside your Unity project to ensure a successfull build.

### When I load the Android Studio project I get an error relating to the "android:theme"?
Please add the following to your Application tag inside your manifest. This is because Unity needs to override the theme which the Estimote Indoor Location SDK is trying to take control of.

*tools:replace"android:theme"*

### When I build the Xcode project I get errors relating to missing libraries?
Please ensure you have completed the setup process within Unity (check the Quick Start Guide). This will ensure all libraries are present in your Unity project ready for building the Xcode project.

### On iOS can I change the descriptions for the permissions requests?
This is currently hardcoded inside the application. We are looking into a solution to make this easier to change, but for now please load up the IndoorLocationPostProcess.cs script and edit the usage descriptions as you require.

### Can the plugin do X/Y/Z?
If there is a feature that we have not implemented please contact us using the [support]({{ "/docs/support/" | prepend: site.baseurl }}) page. We are always looking at improving the plugin and support for our users.
