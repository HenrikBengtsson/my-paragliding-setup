# XCTrack

## Backing up XCTrack configuration

To back up your XCTrack settings to a `<date>_<index>.xcfg` file under
`/storage/emulated/0/Android/data/org.xcontest.XCTrack/files/Config/`
on the Poke,

1. Go to 'Preferences',

2. then 'Export & import config' (or 'Testing & Debug' on XCTrack <=
   0.9.8.6), and

3. click 'Export configuration'.

You will get a pop-up window titled 'Export finished' that says
something like "Current XCTrack configuration saved to file
/storage/emulated/0/Android/data/org.xcontest.XCTrack/files/Config/2023-04-25_00.xcfg`.

If you have configured your sharing on your Poke, you could click
'SHARE' to share via, say, Bluetooth or Email.  I don't have sharing
configured, so I click 'CLOSE' at this point.  I use the 'Destiny' app
(<https://f-droid.org/en/packages/com.leastauthority.destiny/>) to
send my settings to my computer.

This will export your airspaces, portrait and landscape page layouts,
pilot and glider names, connected Bluetooth varios, and other types of
preferences set.  Downloaded terrain maps and road maps will _not_ be
part of the exported `*.xcfg`.  Your xcontest.org username and
password will also _not_ exported.



## Restoring XCTrack configuration

To restore previously backed up XCTrack settings,

1. Go to 'Preferences',

2. then 'Testing & Debug', and

3. click 'Import configuration'.

4. Choose an `*.xcfg` file to import (either among the listed ones or
   under 'OTHER...')

5. Confirm 'Really import configuration?' by pressing YES.

6. Confirm 'Shut down XCTrack?' by pressing YES.

7. In the XCTrack 'App info' display, click 'FORCE STOP', and then
   confirm by pressing 'OK'.

8. Reopen XCTrack.




## Importing partial XCTrack configuration

It is possible to prune an exported XCTrack configuration file such
that not all settings are changed when imported.  This makes it
possible to share parts of your settings with others without them
overriding their other settings such as pilot name and a configured
vario.

For example, the landscape display that I use on my Poke 3 is
available in [xctrack/xcfg/poke3_layouts_landscape.xcfg].  To apply
this to your XCTrack,

1. Backup your current XCTrack settings (see above)

2. Download the XCFG file to your Poke (e.g. using the NeoBrowser app)

3. Import the XCFG file to XCTrack (see above)

After restarting XCTrack, make sure 'Preferences' -> 'Display' ->
'Orientation' is set to either 'Landscape' or 'Reverse Landscape'.
You should now have a the same landscape layout as seen in the photo
of my flight deck.


[xctrack/xcfg/poke3_layouts_landscape.xcfg]: https://github.com/HenrikBengtsson/my-paragliding-setup/blob/develop/xctrack/xcfg/poke3_layouts_landscape.xcfg

