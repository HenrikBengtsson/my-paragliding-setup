# XCTrack

## Sharing Pages layout with others

These instructions assumes you run XCTrack 0.9.8.7 (2023-04-26) or
newer.

### Export "Pages" layouts

1. Go to 'Preferences' -> 'Export & Import config'.

2. Click 'Export configuration'.

3. Select 'PAGES ONLY'.

You will get a pop-up window titled 'Export finished' that says
something like "Current XCTrack configuration saved to file
/storage/emulated/0/Android/data/org.xcontest.XCTrack/files/Config/2023-04-30_pages_00.xcfg`.

If you have Sharing apps configured on your device, click 'SHARE' and
select method for sharing this file.  Otherwise click 'CLOSE' and use
other ways to transfer the file under
`/storage/emulated/0/Android/data/org.xcontest.XCTrack/files/Config/`
on the Android device to another device or storage.  If you're using a
ONYX Poke device, you can use 'BOOXDrop'.


### Import "Pages" layouts

If you received a XCTrack configuration file from some one else,
either one that contains their full configuration, or just their pages
configuration, you can import their "pages" settings to your XCTrack
app.

After having downloaded the `*.xcfg` file to the Android device where
your run XCTrack, open XCTrack and:

1. Go to 'Preferences' -> 'Export & Import config'.

2. Click 'Import configuration'.

3. Click 'OTHER ...' (you might see an error message too) 

4. You will now see an Android file-navigator window. Navigate to the
   `*.xcfg` file you wish to import, and click on it.

5. If you're importing a full XCTrack configuration, you will get
   three options:

   * Replace all (all your config and pages will be overwritten)

   * Replace pages only (overwrite your pages and widgets only)

   * Add pages only (nothing will be overwritten, new pages will be
     added after yours)

   Choose either 'Replace pages only' or 'Add pages only'.

6. Click 'CONTINUE'.

7. If you choose anything else than 'Add pages only', you need to
   confirm too. Click 'YES'.

8. You should see 'Configuration successfully imported'. Click 'OK'.

Done.

You can now go back to 'Preferences' -> 'Pages layout' to confirm that
the new pages have been imported correctly.

Also, make sure 'Preferences' -> 'Display' -> 'Orientation' is set to
either portrait or landscape of the pages you want to use.  This is
important, because pages designed in landscape mode will only work
when the XCTrack display is set to be in landscape mode, and vice
versa for portrait mode.



## Backing up and Restoring XCTrack configuration

It's always good to backup your XCTrack settings once in a while.
This is also the easiest way to get started again if you get a new
Android device.


### Backing up all your XCTrack settings

To back up your XCTrack settings to a `<date>_<index>.xcfg` file under
`/storage/emulated/0/Android/data/org.xcontest.XCTrack/files/Config/`
on the Poke,

1. Go to 'Preferences',

2. then 'Export & import config' (or 'Testing & Debug' on XCTrack <=
   0.9.8.6), and

3. click 'Export configuration'.

You will get a pop-up window titled 'Export finished' that says
something like "Current XCTrack configuration saved to file
/storage/emulated/0/Android/data/org.xcontest.XCTrack/files/Config/2023-04-30_backup00.xcfg`.

This will export your airspaces, portrait and landscape page layouts,
pilot and glider names, connected Bluetooth varios, and other types of
preferences set.

Importantly, downloaded terrain maps and road maps will _not_ be part
of the exported `*.xcfg`.  Your xcontest.org username and password
will also _not_ exported.


If you have configured your sharing on your Poke, you could click
'SHARE' to share via, say, Bluetooth or Email.  I don't have sharing
configured, so I click 'CLOSE' at this point.  I use the 'Destiny' app
(<https://f-droid.org/en/packages/com.leastauthority.destiny/>) to
send my settings to my computer.


### Restoring XCTrack configuration

To restore previously backed up XCTrack settings,

1. Go to 'Preferences',

2. then 'Export & import config' (or 'Testing & Debug' on XCTrack <=
   0.9.8.6), and

3. click 'Import configuration'.

4. Choose an `*.xcfg` file to import (either among the listed ones or
   under 'OTHER...')

5. Confirm 'Really import configuration?' by pressing YES.

6. Confirm 'Shut down XCTrack?' by pressing YES.

7. In the XCTrack 'App info' display, click 'FORCE STOP', and then
   confirm by pressing 'OK'.

8. Reopen XCTrack.




[xctrack/xcfg/poke3_layouts_landscape.xcfg]: https://github.com/HenrikBengtsson/my-paragliding-setup/blob/develop/xctrack/xcfg/poke3_layouts_landscape.xcfg
