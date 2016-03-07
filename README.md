# AndroidScreenCastWxPy
(C) 2016 by Pascal Bauermeister.

This program casts the screen of an Android device (connected via usb) to a window on your computer.

The present program should *just work*, on any computer [1], with any Android [2] device.

- As it is using screencap via adb, the rate is quite low (a few FPS),
but sufficient for slow-changing apps.

- This is probably the maximum speed one can achieve with ANY
device. Faster solutions require either a rooted Android device
(allowing for e.g. VNC) or that the PC is pretending to be a
Chromecast. 

[1] The computer must have Python 2.7 and adb installed, reachable by your PATH; 
also required is wxPython. All not a big deal if you are a developer. The downside
is that there is currently no Debian, OSX nor Windows install packaging [3].

[2] The device must have USB debugging enabled.

[3] The good side is that there is one single executable file.

## Installing
- See the prerequisites in [1] above.
- Copy `androidscreencast` in a location targeted by your PATH environment variable.

## Usage
```
./androidscreencast
```
  -or-
```
python androidscreencast
```

## Supported platforms
- Any Android device (see [2] above)
- Computer: wherever the said environment (see [1] above) is available. Only tested on Linux so far.
