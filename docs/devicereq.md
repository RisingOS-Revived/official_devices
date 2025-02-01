The use of “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”, “SHOULD NOT”, “RECOMMENDED”, “MAY”, and “OPTIONAL” is per the IETF standard defined in RFC2119.

## Audio
* All devices MUST support audio playback for media content.
* Phones MUST support in-call audio.
* Phones MUST support speaker audio.
* Tablet devices capable of in-call audio/speaker audio MUST support in-call/speaker audio.
* Devices SHOULD support any additional audio configuration inherent to their device (eg. echo cancellation, extra mics, etc).
* All devices MUST support any other audio output supported by their stock OS (eg. headphone jack, USB-C, BT).

## RIL
* All devices with RIL supported in their stock OS MUST support RIL for phone calls & data.
* All devices with RIL supported in their stock OS MUST support emergency calling with a SIM inserted (112/911).
* Data-only devices (defined as devices that have a RIL but do not support telephony stack due to hardware/firmware restrictions) are EXEMPTED from phone & emergency dialing requirements.

## Wi-Fi
* All devices with Wi-Fi supported in their stock OS MUST support Wi-Fi.
* All devices with Wi-Fi MUST report same MAC address as on stock OS.
* All devices with Wi-Fi hotspot capabilities MUST support Wi-Fi tethering.

## USB
* All devices with a USB port MUST support file access via MTP.
* All devices with USB tethering supported on their stock OS MUST support USB tethering.
* All devices with a USB port & Data SHOULD support USB tethering.

## GPS
* All devices with GPS supported in their stock OS MUST support GPS.

## Camera
* All devices with Camera supported in their stock OS MUST support Camera, in both front facing and rear camera configurations.
* All devices with Dual (or more) Rear Cameras SHOULD support all rear cameras.
* All devices with Dual (or more) Front Facing Cameras SHOULD support all front cameras.
* All Camera HAL versions accessible with the device's Camera HAL MUST comply with the Camera and Video Recording requirements.

## Video Recording
* All devices with Video Recording supported in their stock OS MUST support Video Recording, in both front facing and rear camera configurations.

## Fingerprint Sensor
* All devices with a Fingerprint Sensor MUST support the Fingerprint Sensor if the stock OS supports it with Marshmallow or higher Android versions.
* All devices with a Fingerprint Sensor SHOULD support the Fingerprint Sensor if the stock OS supports it for all other Android versions.

## Accelerometer
* All devices with an accelerometer MUST support the accelerometer.

## Gyroscope
* All devices with a gyroscope MUST support the gyroscope.

## Proximity
* All devices with a proximity sensor MUST support the proximity sensor.

## Light
* All devices with a light sensor MUST support the light sensor.

## Other Sensors
* All other sensors supported by a device’s stock OS SHOULD be supported.

## SELinux status
* All devices MUST be configured for SELinux Enforcing. Exceptions MAY be made for this.

## Additional Features
* All devices SHOULD support LiveDisplay. Exceptions MAY be made for this.

## Authorship
* All commits MUST have proper authorship to the author of the commits.

## Licenses
* Your used kernel MUST be open source.

## Stability
* If your build is deemed unstable by the team you may not be allowed to maintain officially.

## Exceptions
* Exceptions MAY be made for some of these mentioned requirements.

This document uses work from LineageOS' [device support requirements](https://github.com/LineageOS/charter/blob/master/device-support-requirements.md) which is licensed under CC-BY-3.0, some modifications were made to it.