# CPX Redundancy
#### Purpose
Statement of Work Template intended for Datacenter Volunteer Lead Community Engagements.  

#### Materials
1 AAA Battery housing

6 AAA Batteries (3 spare)

1 Circuit Playground Express

Data/Sync USB Cable


#### Before
Test the equipment Start Procedure below and note any failures or missing items as described in After Procedure below.  For help, use the Get Help information below.  Internet access will be required to download the CPX program.

#### Start
Read through  [Source 1](#Source-1) below. When you are ready, move the image ([Source 2](#Source-2)) to the CPX.  Use instructions located here: [Source 2](#Source-2).  Test the program.

#### Get Ready
**Prep the CPX** : Connect the USB-A/MicroUSB cable to the computer USB port.  Connect the MicroUSB end to the CPX.  Press the reset button twice, like a double-click.  A CPLAYBOOT drive should appear.  Use the information in Program 1 to add the bootloader to the CPX as in [Source 2](#Source-2). 

**Power the CPX**: Insert the batteries into the battery pack.  Connect the battery pack to the CPX. Power on the battery pack.

#### Go
This program contains three elements:

1. Programming the CPX Bootloader to work with MakeCode Bootloader
2. Using the light sensor to read the intensity of the light
3. When light is not detected, sound an alarm

See  [Appendix](#Appendix) for Details. Use the [Lesson](#Lesson) information to explain the lab to relatable concepts at the Datacenter.

#### After
Note any items that are damaged, not working, or missing (including consumables) as noted in Get Help below.

#### Source
1. IR Tag and Reset are all programmed through Makecode.adafruit.com. See [Program 1](#Program-1) below for programming details.

#### Get Help
For any questions contact the Microsoft Datacenter Community Development team at dc-stem@microsoft.com

#### <a id="Appendix"></a>Appendix
Once the Circuit Playground Express (CPX) is connected, shine a bright light on the light sensor near 👁. 
Then connect the battery pack and switch the power to on.
When the CPX is running the program, all LEDs will display green. 

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/greenfive.png"
            /> 
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br><br></br>

When the light source is disrupted from the CPX sensor, all LEDs will display red and a siren alarm will begin.  Each will continue until the light source is returned.

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/redlights.png"
            /> 
<br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br>
<br></br>
<br></br>
<br></br>
<br></br>

A CPX not powered.

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/nopowercpx.jpg"
            /> 
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>

#### <a id="Lesson"></a>Lesson
The purpose of this hands-on STEM lab is to educate the community about Datacenters.  The lights and actions may not exactly replicate, but loosely relate to operations at a datacenter.

#### What:
This lab demonstrates security intrusion and can be used to explain Cyber Security or Physical Security.  

#### Details:
Security is imperative concerning the data that is housed on any of Microsoft Datacenter servers.  Not only do we have the highest cyber security protocols, we also have secure facilities that require appropriate level badge access.  We also take precautions to avoid piggy-back entry into buildings.  Piggy-back entry is a term that may need to be explained.  (One gains entrance when closely entering in after a person in front has scanned and gain access to the building.  The second person does not need to scan their badge.)

#### Share:
When you take a photo and save it to your cloud storage account, you are trusting the file will not be shared to others without your permission.  Certain security protocols are created and practiced to avoid security risks.  Similarly, datacenter buildings are secured to keep data vulnerabilities.  Employees also have different levels of access depending upon job needs.

NOTE:

The labs works by measuring the intensity of the light read by the circuit.  If the light intensity falls below a certain value, an alarm will sound and the LEDs will turn red indicating a breach.

To turn off the alarm, simply restore the light source.  To reset the program, press the reset button on the CPX.

#### <a id="Source-1"></a> Source 1 
The Adafruit Circuit Playground Express (CPX) is a microcontroller with more power, storage space, and RAM than a 386 Intel Computer.  It includes temperature, light, sound, and accelerometer sensors, 10 built in LEDS, speaker, two push buttons, one slide switch, IR receiver and transmitter, 8 analog inputs, power output, 7 capacitive touch inputs, green "ON" LED, reset button, ATSAMD21 ARM Cortex M0 Processor, 2 MB of SPI Flash storage, and a Micro USB port for programming and debugging.

**Source**:
https://learn.adafruit.com/adafruit-circuit-playground-express
[i386 - Wikipedia](https://en.wikipedia.org/wiki/I386?msclkid=d82996eac23711eca097ba0148e8ca79) https://en.wikipedia.org/wiki/I386?msclkid=d82996eac23711eca097ba0148e8ca79 

There are three ways to program the CPX:

1. makecode.adafruit.com
2. CircuitPython
3. Arduino

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

Copy the saved UF2 file from the Intrusion folder and paste it on the CPLAYBOOT root drive.

The CPX lights will flash, then reset and the CPLAYBOOT drive will disappear from the drive list.

The program is now installed

Press the reset button on the CPX.

Once the Circuit Playground Express (CPX) is connected, shine a bright light on the light sensor near 👁.

Then connect the battery pack and switch the power to on.

When the CPX is running the program, all LEDs will display green. 

To **troubleshoot** the CPX device and program:

1. Check the batteries
2. Press reset button 1 time.  This will reset the device, like a computer reboot/restart.
3. Follow steps in Source 1 to download the program to the CPX device.
4. Try another device and see if the problem repeats.  If it repeats check program in Source 1 and 2 to install the program again.
5. Follow the procedure in [Source 3](#Source-3) below to reset to factory settings.  Then repeat the procedure to install the TrioCombo program.

#### <a id="Source-3"></a>Source 3
**Download** the original CPX **bootloader**, navigate to [UF2 Bootloader Details | Adafruit Feather M0 Express | Adafruit Learning System](https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details) [https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details](https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details). Scroll to the bottom of the page and click on the green rectangle, with Circuit Playground Express V#.#.# update-bootloader.uf2.  Click on the link (make sure it is for the Circuit Playground Express).  The file will download.

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
To **create this program**, open [MakeCode.adafruit.com.](https://microsoft.sharepoint.com/teams/TeamDocumentSharing/Shared Documents/STEAM Kit/Intrusion/MakeCode.adafruit.com)  Create the bootloader file by creating the block code program below:

<img style={{margin: "0", clear: "right", float: "left", width: "300px"}}
            src="/images/bootloader.png"
            /> 
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br><br></br>

Program the CPX as listed in [Source 1](#Source-1).
