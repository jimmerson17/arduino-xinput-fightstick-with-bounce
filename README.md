# arduino-xinput-fightstick

# Intro
Needed an XInput script for my custom sticks, found the DaemonBite Arcade Encoder but it was HID and not XInput.  Luckily omgdanieltam already did the footwork, and I just threw Bounce2 at it since I was getting double inputs in some instances (Pegasus FE navigation).

My version requires the Bounce2 library.  I only added bounce code for the directions since that's all I needed.  I'm sure there's a more elegant and less ugly way to do this but it works for me and I don't see any impact on gameplay or responsiveness.

See omgdanieltan's original code and readme for full notes.

# Sources 
DaemonBite Arcade Encoder (https://github.com/MickGyver/DaemonBite-Arcade-Encoder)  
ArduinoXInput Library (https://github.com/dmadison/ArduinoXInput)  
OMGDanielTam's original code (https://github.com/omgdanieltam/arduino-xinput-fightstick)  
Bounce2 Library (https://github.com/thomasfredericks/Bounce2)
