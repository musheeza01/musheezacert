# UART Activating Light Sensor to Show Redundancy
---
### *Information*
---

This document provides the procedure to use the CircuitPython Language to code Circuit Playground Express devices to transmit and receive data.  The project is located here: 

[https://learn.adafruit.com/uart-communication-between-two-circuitpython-boards/code](https://learn.adafruit.com/uart-communication-between-two-circuitpython-boards/code) and here: [Code | UART Communication Between Two CircuitPython Boards | Adafruit Learning System](https://learn.adafruit.com/uart-communication-between-two-circuitpython-boards/code)

Detailed information on Circuit Playground Express can be found here: [The Circuit Playground | Code.org](https://code.org/circuitplayground) or [https://code.org/circuitplayground](https://code.org/circuitplayground)

There are three ways to code the Circuit Playground Express.  This document will detail using CircuitPython to program the Circuit Playground Express device.  The three ways that Circuit Playground Express devices can be programmed are as follows:

1.	makecode.adafruit.com

2.	CircuitPython

3.	Arduino IDE 

---
### *Required Parts*
---

*	At least two Circuit Playground Express Devices (For Redundancy – at least three)

*	Three alligator wires or MiniGrabber wires per pair of Circuit Playground Express devices

*	1 USBA to MiniUSB cable per Circuit Playground Express Devices

---
### *Setup Procedure*
---

Download the latest **stable** release CircuitPython UF2 Installer File, located here: [Circuit Playground Express Download (circuitpython.org)](https://circuitpython.org/board/circuitplayground_express/) or here:

[https://circuitpython.org/board/circuitplayground_express/](https://circuitpython.org/board/circuitplayground_express/)

NOTE:

Once this has been installed, the Circuit Playground Express BOOT drive will change from CPLAYBOOT or FEATHERBOOT to CIRCUITPY. Now you are ready to add the Python programming files.  Which allows python programming files to be added to the boot drive to run the UART program as in the link at the beginning of the document.  This procedure should be followed or the program will not work.

Connect the Circuit Playground Express to the USB drive of the computer with a data sync USB cable (included in the Circuit Playground Express Education Kit).

Double-click the small Reset button in the middle of the CPX, you will see all of the LEDs turn green. If they turn all red, check the USB cable, try another USB port, etc.  Then double-click the small Reset button in the center of the CPX again.  Once the lights all turn green, proceed to the next step.  (If double-clicking doesn't do it, try a single-click!)

<img style={{margin: "0", clear: "right", float: "left", height:"300px", width: "300px"}}
            src="/images/turnoncpx.png"
            /> 
<img style={{margin: "0", clear: "right", float: "left", height:"300px", width: "300px"}}
            src="/images/greencpx.jpg"
            /> 
<br></br><br></br>
            <br></br><br></br>
            <br></br><br></br>
            <br></br><br></br>
            <br></br><br></br>

Next, you should see a new disk drive appear called CPLAYBOOT
Copy the CircuitPython UF2 Installer File to the CPLAYBOOT drive.

The CPLAYBOOT drive will disappear and a new disk drive will appear called CIRCUITPY.  This verifies that the CircuitPython OS has been installed.

---
### *Install the Program*
---

To use the UART Light Sensor Program, Download the Project Bundle located on the project page above in the Information Section or here: 
[https://learn.adafruit.com/pages/22817/elements/3101703/download?type=zip](https://learn.adafruit.com/pages/22817/elements/3101703/download?type=zip)
Unzip the file as a folder. 

This will download three files and one folder.  Open the CIRCUITPY drive.
Rename code.py to oldcode.py
Copy the code.py file from the downloaded bundle UART Light Sensor Program to the Root directory on the CIRCUITPY drive.
Open the lib directory.
Copy the lib\adafruit_pixelbuf.mpy and lib\neopixel.mpy files to the Root\lib directory on the CIRCUITPY drive.

Repeat the steps Setup Procedure and Installing the Program. for each Circuit Playground Express.

---
### *Connect the Devices*
---

Wire the Circuit Playground Express devices such that:

RX pairs to TX

TX pairs to RX

GRD pairs to GRD

If RX – RX or TX to TX – this will not work.  The devices are coded to look for and then act when a signal is received or transmitted on the RX or TX port respectively.


<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/RXTX.png"
            /> 
            
<br></br><br></br>
            <br></br><br></br>
            <br></br><br></br>
            <br></br><br></br>
            

Once all are complete:

Press the reset button once on each Circuit Playground Express. Each should display one single green LED light.  The device is ready to test.

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/cpxled.png"
            /> 
            
<br></br><br></br>
            <br></br><br></br>
            <br></br><br></br>
            <br></br>


________________________________________________________________________________________
### *Test the Program*
________________________________________________________________________________________

Use a flashlight or phone flashlight app to shine the light over the eye sensor.  Depending on the brightness of the light determines the number of LEDs light in order on the connected / paired Circuit Playground Express.

If more than two are connected, try to disconnect one to test redundancy.

Continue to test and play.  When complete, disconnect all MiniGrabbers or Alligator Clips.  Then disconnect from the USB port.  Pack everything away in its proper place.
