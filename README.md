# Windows

1) Plug in the Feather using a Micro USB cable.

2) Quickly press the button on the Feather twice (any button). You should see a red LED pulsating slowly.

3) Open a command prompt by pressing Windows-R, typing "cmd" and then enter.

4) Change directories to where you downloaded and unzipped the "emergency" archive. This is probably in your Downloads directory, something like:

   cd
   cd Downloads/emergency

Might do the trick. You can find this in explorer.

5) Type "ports.cmd" and then enter and look for the word "Adafruit Feather M0". On the same line as that you'll see the text "COM##" where ## are one or two numbers.

6) Type "upload.cmd COM##" where those numbers match the above and press enter. You should see some garbage flow by, ending with:

Verify successful
done in 0.097 seconds
CPU reset.
readWord(addr=0)=0x20007ffc
readWord(addr=0xe000ed00)=0x410cc601
readWord(addr=0x41002018)=0x10010305
writeWord(addr=0xe000ed0c,value=0x5fa0004)

And the Feather should no longer be pulsating.

# Mac OSX

1) Plug in the Feather using a Micro USB cable.

2) Quickly press the button on the Feather twice (any button). You should see a red LED pulsating slowly.

3) Open a terminal by using the finder to open Applications and then Utilities and then double clicking on Terminal.

4) Change directories to where you downloaded and unzipped the "emergency" archive. This is probably in your Downloads directory, something like:

   cd
   cd Downloads/emergency

Might do the trick. You can find this in explorer.

5) Type "bash ports" and look for a line that begins with cuS.usbmodemSTUFF where STUFF is some random looking text and numbers.

6) Type "bash upload cu.usbmodemSTUFF" with the matching text from the line you found above. You should see some garbage flow by, ending with:

Verify successful
done in 0.097 seconds
CPU reset.
readWord(addr=0)=0x20007ffc
readWord(addr=0xe000ed00)=0x410cc601
readWord(addr=0x41002018)=0x10010305
writeWord(addr=0xe000ed0c,value=0x5fa0004)

And the Feather should no longer be pulsating.
