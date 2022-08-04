# moving-robot-arm-by-STT

This repository is about using web serial Api to move a robot arm using esp32.
It works as Follow:

first in the HTML website we have added the WebSerial Api and attached it to the button "connect". when its clicked , it prompts the user to select a serial device (such as our ESP32).

Then when it is connected, it opens a serial port to read and write data from and to the device. When the user speechs a certain word such as "right" the api will store it in a variable named "Right" otherwise will ignore it.

After that in our Arduino Ide we will open the same port and add the required codes to which will take our variable such as "Right" and then move the arm accordingly.
