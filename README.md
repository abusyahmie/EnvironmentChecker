# EnvironmentChecker

### Building Apps with Environment Sensor

This article was written by Sue Smith and can be found at the following link:

`http://code.tutsplus.com/tutorials/building-apps-with-environment-sensors--pre-46879`

Here's the excerpt from the article:

Learn how to use the Android Environment Sensors to detect information about the user's environment, including ambient temperature, pressure, humidity, and light.
The Android system supports a range of device Sensors, some implemented in hardware and some in software. The Environment Sensors are all hardware features, providing access to information about ambient temperature, pressure, humidity, and light. These sensors return values as follows: temperature is measured in degrees Celsius, atmospheric pressure in hPa millibars, relative ambient air humidity as a percentage value, and ambient light in SI lux units. In this tutorial, we will run through the basic process for using these four main Environment Sensors. We will not be using the device temperature sensor, as it is now deprecated as of Android 4.0.

There are many possible applications for these sensors, such as barometers and thermometers. You may have come across such apps in Google Play already, but it is worth noting that they may not necessarily be implementing their functions using Environment Sensors. For example, weather apps often use location data fetched over the Web to determine environment information based on where you are.

Since these sensors are provided via users' hardware, support does vary between devices and manufacturers. At the time of writing, very few Android smartphones or tablets support all of the Environment Sensors, but many of the more recent models support one or more of them. It is vital to carry out checks on whether the user has particular sensors and to avoid using functionality that is totally reliant on them. The only exception to this is if you ensure only users with the required hardware can download your application - you can do this using the filters for an app as listed in the Google Play store.

Note:

1. Added few lines of code in the onAccuracyChanged method to specify which sensor.

2. Tested on my Samsung Galaxy S4 and it worked!
