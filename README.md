pulltrigger
===========

A Raspberry pi C / python / PHP library to pull a trigger on a Raspberry Jolt.

More info here:  
http://jordanbalagot.com/blog/2013/02/26/raspberry-jolt-my-mini-nerf-gun-robot/

https://www.youtube.com/watch?v=9WOxRIo8AGI  

You will need the Adafruit 16 Channel Servo Library, available here: https://learn.adafruit.com/adafruit-16-channel-servo-driver-with-raspberry-pi/using-the-adafruit-library

Place the files from public_html into your /var/www directory.

To run the servo that controls the servo:
Navigate to http://raspberrypi.local/pulltrigger.php

To shut down the pi:
Navigate to http://raspberrypi.local/shutdown.php

pulltrigger.php calls pulltrigger, which is a c script that sudos as root and calls pulltrigger.py, which turns the servo for 1 second and the sets it back to home position. Shutdown.php runs similarly.
