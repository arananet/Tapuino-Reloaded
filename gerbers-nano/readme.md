## Tapuino Reloaded using Arduino Nano.

## Possible fix for 'Card not initialized'

There might be a problem with pin 8 on the SD card buffer. If PCB manufacturer does not populate a required via to make pin 8 from the HC4050 to GND, this could produce a problem with SD card detection. To fix this, try to solder pin 8 to pin 2 of the octocoupler (GND). See the next picture for illustration purposes.

Thanks to the user <b>Alleged-Geek<b/> for point this out.

<img src="https://github.com/arananet/Tapuino-Reloaded/blob/master/images/tapufix.png?raw=true" width="500">
