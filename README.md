TouchSoftly
===========

Proof of concept of screen overlay intercepting touches from a background service.

It has settings in which it can auto-start on boot, this kick auto-start launches a service in the background, and intercepts the touch events and "tries" to inject into an activity.
It can be done by using the main activity, just hit Home key, to bring it into background, the service will continue to run, if you end the activity, service stops.

Sadly, the app cannot be distributed in normal fashion a la 'adb install' etc, due to the way the security is, (its a good thing right?).

Events cannot be injected into an activity.

BUT: If the app was signed with the same keys used in the signing of the ROM then it will work. :)

Distributed under the DWTFYL license :)

Author: t0mm13b.
Date: July 8th, 2012.

Reference: http://android.stackexchange.com/questions/25090/cant-scroll-using-hands-are-there-other-options
