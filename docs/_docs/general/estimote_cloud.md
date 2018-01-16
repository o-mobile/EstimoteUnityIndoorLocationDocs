---
title: Estimote Cloud SDK
permalink: /docs/estimote_cloud/
---

You can enable support for the Estimote Cloud SDK by enabling the feature within the EstimoteUnity inspector under the "Estimote Cloud" section. You will need to provide an App ID and App Token which can be created on the [Estimote Cloud Portal](https://cloud.estimote.com/). There is a handy link within the inspector to take you there.
Once you have enabled the Estimote Cloud support you can request extra information from a beacon using the GetBeaconCloudDetails() method within the EstimoteUnity class.

**NOTE**: You can only use the Estimote Cloud features if you are using Estimote Beacons. Trying to request these details from a non Estimote beacon will fail.
