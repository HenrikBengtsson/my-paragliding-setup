# Mirkit Baofeng HAM radio UV-5R MK4 8W

* https://chirp.danplanet.com/projects/chirp/wiki/Home
* https://wayneoutthere.com/2013/08/31/how-to-program-your-baofeng-uv-5r-with-ubuntu/
* http://marcusjenkins.com/baofeng-uv-5r-programming-under-ubuntu-12-04/


## Program radio via USB cable

## Setup CHIRP

```sh
$ wget https://trac.chirp.danplanet.com/chirp_daily/LATEST/chirp-daily-20211221.flatpak
$ sudo flatpak install chirp-daily-20211221.flatpak 
Required runtime for com.danplanet.chirp/x86_64/master (runtime/org.freedesktop.Platform/x86_64/19.08) found in remote flathub
Do you want to install it? [y/n]: y
Installing in system:
org.freedesktop.Platform/x86_64/19.08             flathub                      a85bd015f173
org.freedesktop.Platform.GL.default/x86_64/19.08  flathub                      54eadc8792db
org.freedesktop.Platform.Locale/x86_64/19.08      flathub                      82c2332b3e80
org.gtk.Gtk3theme.Ambiance/x86_64/3.22            flathub                      73fed99df212
org.freedesktop.Platform.VAAPI.Intel/x86_64/19.08 flathub                      86a7fe067ae4
org.freedesktop.Platform.openh264/x86_64/2.0      flathub                      73f998362a6f
com.danplanet.chirp/x86_64/master                 com.danplanet.chirp-3-origin 168fd65053cc
  permissions: ipc, network, wayland, x11, devices
  file access: home
Is this ok [y/n]: y
Installing: org.freedesktop.Platform/x86_64/19.08 from flathub
```


## First test

Identify /dev/tty? for radio:

1. Turn off radio
2. Unplug the red MERKIT USB programming cable
3. `before=$(ls /dev/tty*)`
4. Plug in the red MERKIT USB programming cable
5. `after=$(ls /dev/tty*)`
6. `diff <(echo "$before") <(echo "$after")` => e.g. `/dev/ttyUSB0`

Run CHIRP:

1. Turn on radio on max volume
2. `chirpw`
3. Menu 'Radio' -> 'Download from radio'
4. Port: `/dev/ttyUSB0`, Vendor: `Baofeng`, Model: 'UV-5R'


