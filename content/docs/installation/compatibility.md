# CPX IR Tag and DC Light Signals
#### Purpose
Statement of Work Template intended for Datacenter Volunteer Lead Community Engagements.  

#### Materials
2 AAA Battery housing

9 AAA Batteries (3 spare)

2 Circuit Playground Express

Data/Sync USB Cable


#### Before
Test the equipment Start Procedure below and note any failures or missing items as described in After Procedure below.  For help, use the Get Help information below.  Internet access will be required to download the CPX program.

### Start
Read through  [Source 1](#Source-1) below. When you are ready, move the image ([Source 2](#Source-2)) to the CPX.  Use instructions located here: [Source 2](#Source-2).  Test the program.

#### Get Ready
**Prep the CPX** : Connect the USB-A/MicroUSB cable to the computer USB port.  Connect the MicroUSB end to the CPX.  Press the reset button twice, like a double-click.  A CPLAYBOOT drive should appear. Use the information in [Program 1](#Program-1) to add the bootloader to the CPX as in [Source 2](#Source-2). 

**Power the CPX**: Insert the batteries into the battery pack.  Connect the battery pack to the CPX. Power on the battery pack.

#### Go
This program contains three elements:

1.	IR Tag ‘laser’ transmitted (Button B)

2.	Reset lights, tag count (Button A)

See  [Appendix](#Appendix) for Details. Use the [Lesson](#Lesson) information to explain the lab to relatable concepts at the Datacenter.

### After
Note any items that are damaged, not working, or missing (including consumables) as noted in Get Help below.

### Source
1.	IR Tag and Reset are all programmed through Makecode.adafruit.com. See [Program 1](#Program-1) below for programming details.

### Get Help
For any questions contact the Microsoft Datacenter Community Development team at dc-stem@microsoft.com

#### <a id="Appendix"></a>Appendix
Pressing the A button (left button when battery adapter is facing down) will reset the IR tag count and set all lights to blue.

<img style={{margin: "0", clear: "right", float: "left", height: "300px", width: "300px"}}
            src="/images/bluelights.jpg"
            /> 
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br>

IR Tag is played by pressing the B button to transmit (TX) the signal to an opposing CPX where the signal will be received (RX).  The ‘pew-pew’ sound is heard when the button is pressed (think Atari Asteroid game).  The dying sound is heard when the IR signal is received by the opposing device (think Atari and last life).  Blue lights indicate not yet hit/tagged or game reset.  Red lights indicate hit/tagged.

<img style={{margin: "0", clear: "right", float: "left", height: "300px", width: "300px"}}
            src="/images/redlights.png"
            /> 
<img style={{margin: "0", clear: "right", float: "left", height: "300px", width: "300px"}}
            src="/images/bluelights.jpg"
            /> 
<br></br><br></br><br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br>
<br></br>
<br></br>


#### <a id="Lesson"></a>Lesson
The purpose of this hands-on STEM lab is to educate the community about Datacenters.  The lights and actions may not exactly replicate, but loosely relate to operations at a datacenter

### What:
This lab demonstrates light signals as a method to alert problems in a Datacenter Colo.  

#### Details:
Explaining a Colo may not be needed, however, explaining the significance of lights is more important.  Pressing B sends an IR signal.  If the receiving CPX board receives the signal, lights turn to red and a sound is heard.  When Button A is press, the IR Tag count is reset and the lights return to blue.

### Share:
Lights give us different signals in the world around us.  Crosswalk lights, stop lights, self-checkout register lights, even car brake lights give us signals for what is ahead.  When you are ‘tagged’ with the IR Signal, the lights on your CPX turn red and emit a sound alerting you that you have just lost the game.  Datacenters have the same alerts.  If a server has a red light, there is a device failure that must be resolved, or you may not be able to retrieve your photo from your Cloud drive on your phone (any relatable example).  

 There are also larger fans that cool Colos by removing heat from the air and replacing with cooler air.  While the fans will not play an audible tune, they may change sounds if there is an eminent problem of failure.  This allows employees to diagnose problems before the failure occurs.

IR Tag signals us to a security breach.  When you have been tagged, you were sent a signal that was intended to tag you out of a game.  However, your goal was to keep from getting tagged and keep your threat and vulnerabilities low.  When your CPX received the signal, your vulnerability was low, threat was high, and security threshold was breached!  There is one thing that you can do to remove your vulnerability and threat and increase your security level.  What is it?

(Answer: Cover the RX sensor.)  Allow time to test this hypothesis.

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
To **create this program**, open makecode.adafruit.com.  Select New Project.  Add the program block code components as required in [Program 1](#Program-1). Save the file.

To **move the program** to the CPX:

Plug in the CPX via the USB/Micro USB cable.

Press the reset button twice on the CPX.

All Pixel LED lights will turn on / solid green

The on small LED will turn on / solid green

D13 small LED will slowly blink red

A folder will appear as CPLAYBOOT.

This will be very similar to a USB thumb drive in function.

Copy the saved UF2 file and paste it on the CPLAYBOOT root drive.

The CPX lights will flash, then reset and the CPLAYBOOT drive will disappear from the drive list.

The CPX is now ready with the installed program.

If the TrioCombo program is running:

The small LEDs will turn blue.

To **troubleshoot** the CPX device and program:

1.	Check the batteries

2.	Press reset button 1 time.  This will reset the device, like a computer reboot/restart.

3.	Follow steps in Source 1 to download the program to the CPX device.

4.	Try another device and see if the problem repeats.  If it repeats check program in Source 1 and 2 to install the program again.

5.	Follow the procedure in [Source 3](#Source-3) below to reset to factory settings.  Then repeat the procedure to install the TrioCombo program.

#### <a id="Source-3"></a>Source 3
**Download** the original CPX **bootloader**, navigate to [UF2 Bootloader Details | Adafruit Feather M0 Express | Adafruit Learning System](https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details)[https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details](https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details). Scroll to the bottom of the page and click on the green rectangle, with Circuit Playground Express V#.#.# update-bootloader.uf2.  Click on the link (make sure it is for the Circuit Playground Express).  The file will download.

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
To **create this program**, open makecode.adafruit.com.  Select New Project.  Add the program block code components as required below.  Save the file.  Program the CPX as listed in [Source 1](#Source-1).

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/blockcodeprogram.png"
            /> 
            <br></br>
            <br></br>
            <br></br>
            <br></br>
            <br></br>
            <br></br><br></br>
<br></br>
<br></br>
<br></br>

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/infrared.png"
            /> 
<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/buttondown.png"
            />             
<br></br>
<br></br>
            <br></br>
            <br></br>
            <br></br>
            <br></br><br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br><br></br><br></br><br></br><br></br>


Save the program by clicking on the blue Save button.  Then download the file by clicking on the pink download button.  The file will be downloaded to your download location on your computer with the same name as in the Save Box.

<img style={{margin: "0", clear: "right", float: "center", width: "300px"}}
            src="/images/MakeCode_Program08.jpg" />

<br></br><br></br><br></br>
Continue with the procedure in [Source 1](#Source-1) to program the CPX with the new bootloader.
