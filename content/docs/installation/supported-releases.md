# CPX Redundancy
#### Purpose
Statement of Work Template intended for Datacenter Volunteer Lead Community Engagements.  

#### Materials
3 AAA Battery housing

12 AAA Batteries (3 spare)

3 Circuit Playground Express

6 MiniGrabber cables (2 blue, 2 green 2 black)

Data/Sync USB Cable

#### Before
Test the equipment Start Procedure below and note any failures or missing items as described in After Procedure below.  For help, use the Get Help information below.  Internet access will be required to download the CPX program.

### Start
Read through  [Source 1](#Source-1) below. When you are ready, move the image ([Source 2](#Source-2)) to the CPX.  Use instructions located here: [Source 2](#Source-2).  Test the program.

#### Get Ready
**Prep the CPX:** Connect the USB-A/MicroUSB cable to the computer USB port.  Connect the MicroUSB end to the CPX.  Press the reset button twice, like a double-click.  A CPLAYBOOT drive should appear.  Use the information in [Program 1](#Program-1) to add the bootloader to the CPX as in [Source 2](#Source-2).
**Power the CPX:** Insert the batteries into the battery pack.  Connect the battery pack to the CPX. Power on the battery pack.

#### Go
This program contains three elements:

1.	Programming the CPX Bootloader to work with CircuitPython

2.	Using the light sensor to display the intensity of the light

3.	Light intensity is replicated/redundant between two CPX boards

See  [Appendix](#Appendix) for Details. Use the [Lesson](#Lesson) information to explain the lab to relatable concepts at the Datacenter.

### After
Note any items that are damaged, not working, or missing (including consumables) as noted in Get Help below.


**Source**
1.	The redundancy program utilizes Universal Asynchronous Receiver-Transmitter (UART), a serial communication protocol.  See [Program 1](#Program-1) below for programming details.

### Get Help
For any questions contact Kristie Morris at v-kmorris@microsoft.com

#### <a id="Appendix"></a>Appendix
Once the Circuit Playground Express (CPX) is connected and powered, the program will display 1 or 2 green solid lit LEDs. 

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/LED.png"
            /> 
<br></br><br></br>
            <br></br><br></br><br></br><br><br></br><br></br><br></br>


To connect the circuits, connect the following:

RX to TX and TX to RX and GND to GND

(RX – Receive, TX – Transmit, GND – Ground)

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/circuit.png"
            /> 
<br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br>

Once the ‘customer’ sends the data to the Datacenters A and B

(The customer receives the intensity of the light source and transmits that signal to be displayed on each of the other two datacenters.)  Here the light signal is brightest showing all 10 LEDs lit.  However, this is not an indication of the strength of the connection to the data center.  Redundancy is a more important concept to deliver.  The signal is duplicated (redundant) between the two datacenters.


<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/datacenters.png"
            /> 
<br></br><br></br>
            <br></br><br></br><br></br><br></br><br></br><br></br><br></br>

To reset the device, press the small reset button once in the center of the CPX.  A reset is sometimes needed after powering on all devices together.  Each device may need a reset.


<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/cpx.png"
            /> 
<br></br><br></br>
            <br></br><br></br><br></br><br><br></br><br></br><br></br>


A CPX not powered

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/nopowercpx.png"
            /> 
<br></br><br></br>
            <br></br><br></br><br></br><br><br></br><br></br><br></br>


#### <a id="Lesson"></a>Lesson
The purpose of this hands-on STEM lab is to educate the community about Datacenters.  The lights and actions may not exactly replicate, but loosely relate to operations at a datacenter.

#### What:
This lab demonstrates light signals as a method demonstrate redundancy between datacenters.  

#### Details:
The term redundancy may need to be explained.  A good start may be to ask the audience to define redundancy.  Note that Microsoft Datacenters have triple redundancy.

NOTE:
The labs works by measuring the intensity of the light given to the ‘customer’ and then transmitted signal to the redundant datacenters.  It is imperative the cables are connected correctly for this lab to demonstrate the message of redundancy properly.  RX  TX, TX  RX, GND  GND

It is easier to explain if using the same color cables to go out from the Customer CPX to the Datacenters.  As an example:
From Customer:

RX out = Red MiniGrabber Cable

TX out = Green MiniGrabber Cable

GND out = Black MiniGrabber Cable

#### <a id="Source-1"></a> Source 1 
The Adafruit Circuit Playground Express (CPX) is a microcontroller with more power, storage space, and RAM than a 386 Intel Computer.  It includes temperature, light, sound, and accelerometer sensors, 10 built in LEDS, speaker, two push buttons, one slide switch, IR receiver and transmitter, 8 analog inputs, power output, 7 capacitive touch inputs, green "ON" LED, reset button, ATSAMD21 ARM Cortex M0 Processor, 2 MB of SPI Flash storage, and a Micro USB port for programming and debugging.

**Source**:
https://learn.adafruit.com/adafruit-circuit-playground-express
[i386 - Wikipedia](https://en.wikipedia.org/wiki/I386?msclkid=d82996eac23711eca097ba0148e8ca79) https://en.wikipedia.org/wiki/I386?msclkid=d82996eac23711eca097ba0148e8ca79 


There are three ways to program the CPX:

1.	makecode.adafruit.com

2.	CircuitPython

3.	Arduino

This program was created with makecode.adafruit.com.  Makecode is a Microsoft product that allows for block style coding.  The program written for this STEM activity is located below in Program 1.

When the CPX is first connected to a computer with the USB cable, it will run the program that is stored on the device.  This may not be the program that you desire to run.  Follow the procedure in Source 3 to reset the CPX to the factory settings.  The CPX will hold the program and not reset to factory settings upon power off.

#### <a id="Source-2"></a>Source 2
To **create this program**, open learn.adafruit.com/uart-communication-between-two-circuitpython-boards/code.  Scroll down on the page and select Download Project Bundle.


<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/projectbundle.png"
            /> 
<br>

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/projectcode.png"
            /> 
<br></br><br></br>
            <br></br><br></br><br></br><br><br></br>



To move the program to the CPX:

Plug in the CPX via the USB/Micro USB cable.

Press the reset button twice on the CPX.

All Pixel LED lights will turn on / solid green

The on small LED will turn on / solid green

D13 small LED will slowly blink red

A folder will appear as CPLAYBOOT.

This will be very similar to a USB thumb drive in function.

Copy the saved UF2 file from the CPX_OS_to_CircuitPy and paste it on the CPLAYBOOT root drive.  (The UF2 file can be downloaded from circuitpython.org/downloads, select Circuit Playground Express.  Download the most recent Stable Version.  Locate the downloaded file: update-bootloader-circuitplay-m0-v3.7.0.uf2.  Copy this file and paste it into the CPLAYBOOT drive, which is the Circuit Playground Express board)

The CPX lights will flash, then reset and the CPLAYBOOT drive will disappear from the drive list.

The CPX will now appear as a folder called CPYTHON

Rename the code.py file in CPYTHON to oldcode.py

Copy the code.py file from UART-Between-Boards/CircuitPython 7.x  (This will be part of the downloaded project bundle form the top of the page.)

Paste the code.py file into the CPYTHON directory on the CPX

Open the UART-Between-BOARDS/CircuitPython 7.x/lib

Copy the two py files (adafruit_pixelbuf.mpy and neopixel.mpy)

Paste the files in the CPYTHON/lib folder

Press the reset button on the CPX.

If there is 1-2 green solid lit LEDs on the CPX, the CPX is now ready with the installed program.

To troubleshoot the CPX device and program:

1.	Check the batteries

2.	Press reset button 1 time.  This will reset the device, like a computer reboot/restart.

3.	Follow steps in Source 1 to download the program to the CPX device.

4.	Try another device and see if the problem repeats.  If it repeats check program in Source 1 and 2 to install the program again.

5.	Follow the procedure in [Source 3](#Source-3) below to reset to factory settings.  Then repeat the procedure to install the Redundancy program.

#### <a id="Source-3"></a>Source 3
**Download** the original CPX **bootloader**, navigate to UF2 Bootloader Details | Adafruit Feather M0 Express | Adafruit Learning System (https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details). Scroll to the bottom of the page and click on the green rectangle, with Circuit Playground Express V#.#.# update-bootloader.uf2.  

Click on the link (make sure it is for the Circuit Playground Express).  The file will download.


<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/circuitplaygroundexpress.png"
            /> 
<br></br>

To **move the bootloader** to the CPX:

Plug in the CPX via the USB/Micro USB cable.

Press the reset button twice on the CPX.

All Pixel LED lights will turn on / solid green

The on small LED will turn on / solid green

D13 small LED will slowly blink red

A folder will appear as CPLAYBOOT.

This will be very similar to a USB thumb drive in function.

Copy the saved UF2 file (from the above procedure) and paste it on the CPLAYBOOT root drive.

The CPX lights will flash, then reset and the CPLAYBOOT drive will disappear from the drive list.

The CPX is now ready with the original bootloader.

#### <a id="Program-1"></a>Program 1
To **create this program**, open [Code | UART Communication Between Two CircuitPython Boards | Adafruit Learning System](https://learn.adafruit.com/uart-communication-between-two-circuitpython-boards/code). Follow the instructions located at the [link here](https://learn.adafruit.com/uart-communication-between-two-circuitpython-boards/code). Program the CPX as listed in [Source 1](#Source-1).

Continue with the procedure in [Source 1](#Source-1) to program the CPX with Circuit Python.
