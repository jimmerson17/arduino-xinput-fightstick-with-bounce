# arduino-xinput-fightstick

# Intro
Was trying to replace a bad board from a Hori RAP fightstick and was looking for a solution. First came across DaemonBite Arcade Enccoder (https://github.com/MickGyver/DaemonBite-Arcade-Encoder), which I initially tried to hook up. It worked great, but when I tried to play some fighting games, I realized that the button layout was not correct. Some games let you adjust all the layout (ex: Tekken 7), but some did not. 

I then tried to find a different solution and came across an XInput library for Arduinos (https://github.com/dmadison/ArduinoXInput). This made the controller appear to be an XBOX 360 controller, which was ideal, since many games will have XBOX buttons mapped out. Also since this was an HORI RAP XBOX 360/XBOX One fightstick, the art was already correct for what we needed. I also wanted to take advantage of having a switch between the D-Pad and Left-Stick. This allows for greater flexability in games.

# Requirements
(1) Arduino Leonardo (or any boards supported by the ArduinoXInput library)  
(2) Previous fightstick (or all the parts needed for a custom stick [buttons/joystick])  
(3) The ArduinoXInput Library (https://github.com/dmadison/ArduinoXInput)

# Setup
Since I previously was using the DaemonBite Arcade Encoder, the button layout is mapped similarily:

PIN 0 : X  
PIN 1 : Y  
PIN 2 : B  
PIN 3 : A  
PIN 4 : LB  
PIN 5 : D-pad/L-Stick switch  
PIN 6 : LT  
PIN 8 : Left Stick Down  
PIN 9 : Right Stick Down  
PIN 10: RT  
PIN 14: START  
PIN 15: RB  
PIN 16: SELECT/BACK  
PIN A0: UP  
PIN A1: DOWN  
PIN A2: LEFT  
PIN A3: RIGHT  

For all the buttons, you will only need a wire between the PIN and the button, and the other wire between the button and GROUND on the Arduino.

# Uploading Code
You will need to follow the ArduinoXInput library instructinos on how to upload code. (https://github.com/dmadison/ArduinoXInput_AVR). As long as you have the library installed, the code should work just fine.

# Extra
As an added bonus of using your own Arduino, you can change the name of the controller when programming the Arduino by updating the boards.txt file.

# Sources 
DaemonBite Arcade Encoder (https://github.com/MickGyver/DaemonBite-Arcade-Encoder)  
ArduinoXInput Library (https://github.com/dmadison/ArduinoXInput)
