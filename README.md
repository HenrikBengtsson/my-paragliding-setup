# My paragliding gadgets

_Last updated: 2023-01-15_

I've got the following devices on my paragliding cockpit since May
2022:

* Vario: [BlueFlyVario] w/ Bluetooth & GPS v22

* Display: [ONYX BOOX Poke 3] Android 7-inch e-reader running the
  XCTrack app

* Keyboard: [Recoil Waterproof Bluetooth Media Button]

Everything is attached using industrial-strength velcro. In addition
to this, I carry an Android phone in my pocket that shares internet
with the Poke 3 e-reader for XCTrack live location sharing and viewer.

I'm fairly happy with this set up. The readability of the e-reader is
excellent - the brighter the sun is, then better it is, and it's
already awesome on cloud days. The e-reader has a touchscreen, but
since that works so and so with gloves, I use the five-button media
button as an external keyboard. The bluetooth connection between the
Poke 3 e-reader and the BlueFlyVario is 100% reliable and always
automatically. Same with the media button.

The only complaint I have is that the BlueFlyVario has twice refused
to boot up. Unfortunately, when this happens, the _only_ way to get it
working again is to reflash the firmware, but that requires an MS
Windows computer, which you probably don't bring on your flying trip.
This has happend twice to me (August 2022, and December 2022) - both
times during flying trips ¯\_(ツ)_/¯.


## Procedure on launch

1. Power on the Poke 3

2. On Android phone, start WiFi hotspot

3. Confirm that the Poke 3 is connected to the phone's WiFi (must be
   done before starting XCTrack!)

4. Power on the BlueFlyVario vario

5. Start XC Track

6. Confirm that live tracking and GPS works

7. Power on the Media Button and confirm pressing left-right shifts
  XCTrack displays

The only little bit of friction in this set up is the hotspot setup
and making sure the Poke 3 has a wifi connection before launching
XCTrack.  Without that, it's just power on the devices and starting
the XC Track app.


## Gadget details

### Vario: BlueFlyVario with Bluetooth & GPS v22

I've got the [BlueFlyVario] with Bluetooth & GPS v22.  We order two on
2022-05-12 for 348 AUD (~240 USD) and received them 2022-05-29.

* Weight: 48 g

* Dimensions: 58 x 36 x 16 mm

* Battery: ~8 hours (w/ Bluetooth & electromagnetic transducer
  running). 2-3 hours to fully charge

* Power button: click to turn ON, long press to turn OFF

* Power button when already ON: short press toggles audio ON, BUZZER,
  and OFF

* Battery status (during startup):

  1. First beep is a 1.0s beep at 4000 Hz
  2. Followed by 1-6 "battery" beeps (indicating 3.6-4.2 V)
  3. Followed by a short 0.2s beep at 4000 Hz

* LED lights:

  - BLUE (Bluetooth):
  
      + Flash every second => Bluetooth scanning
      
      + Double flash every second => connected
      
      + Solid => Bluetooth module is disabled (settings
        `SecondsBluetoothWait`).  Fix by restarting vario

  - ORANGE (GPS):
  
      + 1.0s flashing => GPS 3D fix
      
      + off => no GPS fix
      
  - GREEN:
  
      + During startup
      
      + When pressing button
      
      + When lift beep sounds (setting `GreenLED`)

  - RED:
  
      + Charging (turns off if full charged, but may stays on for
        trickle charging)

* Track logs:

  - Capacity: ~60 hours at one-second intervals
  
  - Always on: when GPS has 3D fix (ORANGE flash)


### Display: ONYX BOOX Poke 3 Android 10 e-reader

I ordered the [ONYX BOOX Poke 3] e-reader from BestBuy USA on
2022-05-13 for 190 USD and received it on 2022-05-19.

* Weight: 150 g

* Dimensions: 153 x 107 x 6.8 mm

* Android: 10

* Google Play Store: no/maybe (failed to install it)

* Speaker: no

* XCTrack: Install via [APK](https://xctrack.org/Download.html)



## Configuration

### Poke3, BlueFlyVariom and XCTrack

Use BlueFlyVario as external GPS in XTrack:

1. In Poke 3 Bluetooth settings, pair BlueFlyVario device
   (e.g. BlueFly-7D0D). No PIN required

2. In Poke 3, enable 'Location' by click on the map icon (to the very
   right) in the Poke 3 pulldown menu **IMPORTANT**: if this is not
   done, then you cannot connect the BlyFlyVario device in XCTrack

3. In XCTrack, go to 'Preferences', then 'Connections & Sensors'.
   Click 'External sensors', select 'Bluetooth sensor' and click 'OK'.
   It will scan for paired Bluetooh devices. Select the BlueFlyVario
   device (e.g. BlueFly-7D0D).

### BlueFlyVario setting

Options to change hardware settings:

* Android: [BlueFlyVario Android App] (installable on Poke 3)
  Download: <https://blueflyvario.com/files/BlueFlyVario.apk>
    
* Any operating system: [BFV Desktop Java Application]
  Download: <https://blueflyvario.com/files/BFVDesktop0.85.zip>

For Poke 3, which does not have a speaker, change:

* `UseAudioWhenConnected`: `true` (default `false`)


[BlueFlyVario]: https://www.blueflyvario.com/
[BlueFlyVario Android App]: https://www.blueflyvario.com/software/
[BFV Desktop Java Application]: https://www.blueflyvario.com/software/
[Recoil Waterproof Bluetooth Media Button]: https://smile.amazon.com/gp/product/B085BYDHG9/
[ONYX BOOX Poke 3]: https://onyxboox.com/boox_poke3
