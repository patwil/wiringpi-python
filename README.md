[WiringPi](https://github.com/WiringPi/WiringPi.git) is perhaps the most comprehensive and fastest set of C libraries for controlling RPi GPIO.
Unfortunately there is no up-to-date Python version at present which works on 64-bit Arch Linux.

This package is a wrapper to call WiringPi lib routines from Python.

Ensure that WiringPi has been built and installed prior to installing this package using:
```
makepkg -i
```

Test it is installed as follows:
```
python -c 'import WiringPi; print(WiringPi.__file__)'
```
