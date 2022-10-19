# CPX Server Indicator Lights
#### Purpose
Statement of Work Template intended for Datacenter Volunteer Lead Community Engagements.  

#### Materials

1 AAA Battery housing

6 AAA Batteries (3 spare)

1 Circuit Playground Express

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

1.	Programming the CPX Bootloader to work with MakeCode Bootloader

2.  Using three touch capacitors to activate ‘alarms’ shown as light signals on the CPX Board

3.	When three different capacitors are touched, the lights change color from Red, Yellow, Green, or off.

See  [Appendix](#Appendix) for Details. Use the [Lesson](#Lesson) information to explain the lab to relatable concepts at the Datacenter.

### After
Note any items that are damaged, not working, or missing (including consumables) as noted in Get Help below.

#### Source
1.	The program utilizes a simple code in MakeCode. See [Program 1](#Program-1) below for programming details.

### Get Help
For any questions contact the Microsoft Datacenter Community Development team at dc-stem@microsoft.com.

#### <a id="Appendix"></a>Appendix
Once the Circuit Playground Express (CPX) has been programmed and connected to the battery pack, the lights will not be on.  You will see the smaller green LED lit near the word ‘On’.  This shows the device is on and ready to use.  Use caution to not touch the touch capacitors A4, A5, A6, A7 as touching these will activate the program. 


<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/capacitor.png"
            /> 
<br></br><br></br>
            <br></br><br></br><br></br><br></br><br></br><br></br><br></br>

Touching the SCL / A4 labeled capacitor will cause the following to repeat 5 times. (Red lights)

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/redone.png"
            /> 
<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/redfive.png"
            />         
<br></br>
<br></br>
            <br></br>
            <br></br>
            <br></br> 
            <br></br><br></br><br></br>


Touching the SDA / A5 or RX / A6 labeled capacitor will cause the following to repeat 3 times. (Yellow lights)

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/yellowone.png"
            /> 
<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/yellowfive.png"
            />             
<br></br><br></br>
            <br></br>
            <br></br>
            <br></br>
             <br></br>

Or

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/yellow.png"
            /> 
<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/yellowlightsfive.png"
            />             
<br></br><br></br>
            <br></br><br></br><br></br> <br></br>

Touching the TX / A7 labeled capacitor will cause the following to repeat 3 times. (Green lights)

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/green.png"
            /> 
<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/greenfive.png"
            />             
<br></br><br></br>
            <br></br>
            <br></br>
            <br></br>
             <br></br>
             <br></br>
             <br></br><br></br><br></br><br></br>
            
#### <a id="Lesson"></a>Lesson
The purpose of this hands-on STEM lab is to educate the community about Datacenters.  The lights and actions may not exactly replicate, but loosely relate to operations at a datacenter.

### What:
This lab demonstrates light signals as a method of demonstrating light signals and alerts within the datacenters.  

### Details:
The term server or JBOD (just a bunch of disks) may need to be explained.  A good start may be to ask the audience to define server.  We see signals every day.  What things do you see around you that alert you?  Several things in our world alert us or caution us: stop lights, cross walk signals, flashing lights, fire alarms, security alarms, phone ringer, car horn, kitchen timer, and many more.  Servers have lights that alert technicians of their operability.  Green is good. Yellow signifies a problem.  Red signifies a failure.  Some servers have blue lights.  Equipment, like HVAC or heating and cooling systems, have motors with large fans.  As those units run, they make a specific sound.  Failures can be noticed by the change in sound of equipment.  The signals and sounds alert us of eminent failure.  Just like the seconds counting down on a crosswalk signal, lights and sounds notify technicians of issues that need attention.  

NOTE:
This lab works by touching the A4, A5, A6, or A7 touch capacitors on the CPX board.

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
To **create this program**, open makecode.adafruit.com.  Select New Project.  Add the program block code components as required in [Program 1](#Program-1).  Save the file.

To **move the program** to the CPX: 

Plug in the CPX via the USB/Micro USB cable. 

Press the reset button twice on the CPX. 

All Pixel LED lights will turn on / solid green 

The on small LED will turn on / solid green 

D13 small LED will slowly blink red 

A folder will appear as CPLAYBOOT. 

This will be very similar to a USB thumb drive in function. 

Copy the saved UF2 file from the Intrusion folder and paste it on the CPLAYBOOT root drive. 

The CPX lights will flash, then reset and the CPLAYBOOT drive will disappear from the drive list. 

The program is now installed 
 
Press the reset button on the CPX. 

Once the Circuit Playground Express (CPX) is connected, without MiniGrabbers attached, all LEDs will display blue.  

To **troubleshoot** the CPX device and program: 

1.	Check the batteries 

2.	Press reset button 1 time.  This will reset the device, like a computer reboot/restart. 

3.	Follow steps in Source 1 to download the program to the CPX device. 

4.	Try another device and see if the problem repeats.  If it repeats check program in Source 1 and 2 to install the program again. 

5.	Follow the procedure in [Source 3](#Source-3) below to reset to factory settings.  Then repeat the procedure to install the Intrusion program. 

#### <a id="Source-3"></a>Source 3
**Download** the original CPX **bootloader**, navigate to [UF2 Bootloader Details | Adafruit Feather M0 Express | Adafruit Learning System](https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details)[https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details](https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details). Scroll to the bottom of the page and click on the green rectangle, with Circuit Playground Express V#.#.# update-bootloader.uf2.  

Click on the link (make sure it is for the Circuit Playground Express).  The file will download.

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/circuitplaygroundexpress.png" />
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
To create this program, open adafruit.MakeCode.com.  Create the bootloader file by creating the block code program below.  

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/blockcode.png" />
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/blockcodetwo.png" />
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/blockcodethree.png" />
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/blockcodefour.png" />
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>

Program the CPX as listed in [Source 1](#Source-1).

Continue with the procedure in [Source 1](#Source-1) to program the CPX with Circuit Python.
