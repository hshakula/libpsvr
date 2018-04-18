#LibPSVR
C library for Morpheus (Playstation VR). Tested with Ubuntu 15.10 + libusb-1.0.20.

## Build
##### dll/shared object
```
$ make
```
or
```
$ make shared
```
##### library
```
$ make lib
```

## Example
##### using dll/shared object
```
$ make example
```
##### using library
```
$ make example-lib
```

## OS X (El Capitan)
For quick start, use brew before build.  

```
$ brew install pkg-config libusb
```

You will need to unload kernel modules manually.  

```
$ sudo kextunload -b com.apple.driver.usb.IOUSBHostHIDDevice
```

## Windows
Requires the latest libusb to be installed.
To compile, use the solution in the LibPSVR folder.  
Solution file is for Visual Studio 2017.  
  
To use PSVR with this, you must install WinUSB or libusb drivers for the PS VR Sensors and PS VR Control, Interfaces 4 and 5 respectively.  
You can use zadiag, which is referenced with libusb, to install the drivers.