# ONYX Poke Device

## Transfer files

There are several options to transfer files back and forth between a
computer or a smartphone and the Poke device.  I found that the
'BOOXDrop' alternative is quite convenient since it requires no login
or account setup.

I don't think one can transfer these files via the ONYX Cloud Storage;
it looks like you can only store notes and books via the cloud
storage.  See the Appendix for my notes on this.


### BOOXDrop

Each BOOX device runs a built-in web server that can be access by
other devices on the same local network (e.g. on the same WiFi
network). [Comment: I need to figure out how to disable this /Henrik
2023-04-30].  To find the website address for your device,

1. Go to 'Apps'

2. Click 'BOOXDrop' (might be grouped under 'Onyx apps')

That will should you a URL that looks something like
`http://192.168.1.8:8085`, where `192.168.1.8` is the IP number of the
device (yours will be different) on your local network (e.g. WiFi).
The `8085` number at the end is a port number, and we all have the
same one.  If you're lazy to type this in on your phone, you can scan
the QR code.

3. Open your Poke's BOOXDrop URL in your computer's web browser.  Your
   Poke and your computer must be connected to the same local network
   (e.g. WiFi).  This will open up a webpage title 'BOOX Drop' where
   you can browser the files on your Poke, and upload ('Send to BOOX')
   and download ('Save to Computer') files.


## Update firmware

I'm running firmware 2023-04-20_11-32_3.3.2_6c3976585 (last checked
2023-08-15).


## Install apps by APK files

I failed to set up Google App Store on the ONYX Poke 3.  The only way
I found to install apps is by download their APK file.




## Appendix

### Create ONYX Account (optional/not useful)

On Poke 3,

1. Go to 'Settings'.

2. At the very top, click on the icon for 'ONYX Account' ("Get 10GB
   Cloud Storage for Notes Sync and Other Cloud Services").

3. Select 'Servers' (I picked 'EUR(eur.boox.com)' because of EU's
   stricter privacy rules).

4. Scroll down to 'Login Methods' and select the 'Email' icon (so you
   can register without having to give out your phone number).

5. Under 'Email', enter your email address.

6. Click 'Get verification code'

7. Check your email for the six-digit verification code.

8. Enter verification code.

9. Check that you agree on the terms and conditions.

10. Click 'Login'.

You should now be logged into the ONYX account, which you can confirm
by going to the 'Settings' screen. There it should now say '<your
email address>' ("Cloud Storage: 0/10 GB") at the very top.



### Connect to ONYX Cloud Storage from web browser

Each ONYX device gets 10 GB of free cloud storage.  This requires your
to sign up for an account (see Appendix for instructions).

On your computer, or smart phone,

1. Go to your ONYX account server (e.g. <https://eur.boox.com>) in the
   web browser.

2. Enter your login information (e.g. email address).

3. Click 'Obtain Verification Code'.

4. Check your emails for the one-time verification code.

5. Check 'Agree ...'.

6. Click 'Sign in'.

You should now see a website titled 'BOOX' with menu items 'Notes',
'BooxDrop', 'Library' and 'Import Reading'.

_Comments_: It looks like 'BooxDrop' page here also requires your
computer and Poke to be on the same local network. In other words, I
don't think you can transfer files via 'BooxDrop' over the cloud or
via the cloud storage.

