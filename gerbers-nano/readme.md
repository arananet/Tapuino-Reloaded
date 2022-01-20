## Tapuino Reloaded using Arduino Nano.

File description:

tapureloaded_arduinonano.042 last version.

tapureloaded_nano.zip version 0.41.

## Possible fix for 'Card not initialized' on version 0.41

There might be a problem with pin 8 on the SD card buffer. If PCB manufacturer does not populate a required via to make pin 8 from the HC4050 to GND, this could produce a problem with SD card detection. If you have a multimeter, try to measure pin 8 from the HC4050 to GND, if you have continuity then the SD Card detection or initialization problem might be elsewhere, if not, to fix this, try to solder pin 8 to pin 2 of the octocoupler (GND). 

Also do not use CD4050BM it wont work, use HC4050 or HCT4050 instead.

See the next picture for illustration purposes.

Thanks to the user <b>Alleged-Geek<b/> for point this out.

<img src="https://github.com/arananet/Tapuino-Reloaded/blob/master/images/tapufix.png?raw=true" width="500">
