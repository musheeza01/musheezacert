# Soil Tester
#### Purpose
Statement of Work Template intended for Datacenter Volunteer Lead Community Engagements.  

#### Materials
1 AAA Battery housing

6 AAA Batteries (3 spare)

1 Circuit Playground Express

2 Minigrabber test lead cables or Alligator Clip test lead cables

2 large paper clips (2”) – (without plastic coating)

Data/Sync USB Cable

2 cups soil, 1 with plant or 2 potted plants


#### Before
Test the equipment Start Procedure below and note any failures or missing items as described in After Procedure below.  For help, use the Get Help information below.  Internet access will be required to download the CPX program.

### Start
Read through  [Source 1](#Source-1) below. When you are ready, move the image ([Source 2](#Source-2)) to the CPX.  Use instructions located here: [Source 2](#Source-2).  Test the program.

#### Get Ready
**Prep the soil**: Add water to one pot/cup of soil.  Leave the other pot/cup dry.

**Prep the lead cables**: Straighten both paperclips, leaving the outer edge bent at a sweeping 90°.  Insert the batteries into the battery pack.  Connect one end of the black test lead cable to the GND on the CPX.  Connect the other end to a paper clip.  Place the paper clip into the moistened soil. Connect one end of the red test lead cable to the A1 port on the CPX.  Connect the other end of the red test lead cable to the second paper clip.  Insert the paper clip into the dry pot/cup of soil.  

**Power the CPX**: Insert the batteries into the battery pack.  Connect the battery pack to the CPX. Power on the battery pack.

#### Go
The running program will refresh every two seconds.  Let the device come to temperature.  With the battery connector facing straight down, the right-side LEDs will display all red (needs water/not conductive) or all green (has water/conductive).  The lights on the left-side will display the temperature with 2°F increments. See  [Appendix](#Appendix) for Details. Use the [Lesson](#Lesson) information to explain the lab to relatable concepts at the Datacenter.


### After
Note any items that are damaged, not working, or missing (including consumables) as noted in Get Help below.

**Source**
1. https://learn.adafruit.com/soil-moisture-sensor-with-circuit-playground-express?msclkid=c5ab76f9c25211eca9ade6549ce5cca6

2. https://learn.adafruit.com/assets/78944

### Get Help
For any questions contact the Microsoft Datacenter Community Development team at dc-stem@microsoft.com

#### <a id="Appendix"></a>Appendix
<img src="/images/greencircuit.png" style=" float: left;" />
<img src="/images/redcircuit.png" style="margin:30px; float: left;" />
<br></br>
<br></br>
<br></br>
<br></br><br></br>
<p style="text-align: left;">
Moist Soil                 </p>              <p style="margin:110px; margin-top:-28px;">Needs Water </p> 

<br></br>

<img src="/images/c1.png" style="float: left;" />
<img src="/images/c2.png" style="margin-left:30px; float: left;" />
<img src="/images/c3.png" style="margin-left:30px; float: left;" />
<img src="/images/c4.png" style="margin-left:30px; float: left;" />
<img src="/images/c5.png" style="margin-left:30px; float: left;" />
<img src="/images/c6.png" style="margin-left:30px; float: left;" />

<br></br><br></br><br></br><br></br><br></br>
<p style="text-align: left;"> ≤ 60 °F   </p>                          
<p style="margin-left:130px; margin-top:-27px;">61-62°F </p> 
<p style="margin-left:260px; margin-top:-27px;">63-64°F </p> 
<p style="margin-left:380px; margin-top:-27px;">65-66°F </p> 
<p style="margin-left:500px; margin-top:-27px;">67-68°F </p> 
<p style="margin-left:620px; margin-top:-27px;">69-71°F </p> 

<br></br><br></br>

<img src="/images/yellowcircuit1.png" style="float: left;" />
<img src="/images/yellowcircuit2.png" style="margin-left:30px; float: left;" />
<img src="/images/yellowcircuit3.png" style="margin-left:30px; float: left;" />
<img src="/images/yellowcircuit4.png" style="margin-left:30px; float: left;" />
<img src="/images/yellowcircuit5.png" style="margin-left:30px; float: left;" />
<br></br><br></br><br></br><br></br><br></br>

<p style="text-align: left;"> ≤ 60 °F                 </p>             
<p style="margin-left:130px; margin-top:-27px;"> 72-73°F </p> 
<p style="margin-left:260px; margin-top:-27px;"> 74-75°F </p> 
<p style="margin-left:380px; margin-top:-27px;"> 76-77°F </p> 
<p style="margin-left:500px; margin-top:-27px;"> ≥ 80°F </p> 


#### <a id="Lesson"></a>Lesson
The purpose of this hands-on STEM lab is to educate the community about Datacenters.  The lights and actions may not exactly replicate, but loosely relate to operations at a datacenter.

### What
This lab tests the moisture (conductivity) and temperature.  

### Details
The moisture test is a test of conductivity.  When the soil is dry (or not grounded with the second wire) the light is red, alerting the audience to a problem.  Just like the lights on the servers in a datacenter rack, a red light is an indicator of failure.  This indicator means there is an immediate issue that needs to be resolved.

The temperature test gives the ambient temperature by every 2°F.  See [Source 2](#Source-2) for specifics.  The datacenters create lots of heat with the equipment running and must be cooled.  Microsoft is committed to using 100% renewable energy by 2030.  Temperature is an important factor, just like August heat or January cold is to our bodies.

### Share
Lights give us different signals in the world around us.  Crosswalk lights, stop lights, self-checkout register lights, even car brake lights give us signals for what is ahead.  When this plant does not have enough water, the lights turn red.  When the plant has enough water, the lights turn green.  If it is too cold, the lights are blue.  If the plant is too warm, the lights are yellow.  Datacenters have the same alerts.  If a server has a red light, there is a device failure that must be resolved, or you may not be able to retrieve your photo from your Cloud drive on your phone (any relatable example).  We also have a commitment to remove the carbon by 2030 that we have put into the environment since 1975 and become carbon negative.  Carbon negative means we will remove more carbon than we have emitted in our energy consumption.  We are also committed to renewable energy goals.

<img src="/images/progress.jpg" style="height: 70%; width: 70%; float: left;" />
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br>

### Source:
https://blogs.microsoft.com/blog/2022/03/10/an-update-on-microsofts-sustainability-commitments-building-a-foundation-for-2030/ 

#### <a id="Source-1"></a> Source 1 
The Adafruit Circuit Playground Express (CPX) is a microcontroller with more power, storage space, and RAM than a 386 Intel Computer.  It includes temperature, light, sound, and accelerometer sensors, 10 built in LEDS, speaker, two push buttons, one slide switch, IR receiver and transmitter, 8 analog inputs, power output, 7 capacitive touch inputs, green "ON" LED, reset button, ATSAMD21 ARM Cortex M0 Processor, 2 MB of SPI Flash storage, and a Micro USB port for programming and debugging.

#### Source:
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

If the soil tester program is running:

The small on LED will turn on / solid green

Right side – LEDs will turn on / solid red (if not grounded)

Left side – LEDs will turn yellow or blue, depending on ambient room temperature (see Appendix)

To troubleshoot the CPX device and program:

1.	Check the batteries

2.	Press reset button 1 time.  This will reset the device, like a computer reboot/restart.

3.	Follow steps in Source 1 to download the program to the CPX device.

4.	Try another device and see if the problem repeats.  If it repeats check program in Source 1 and 2 to install the program again.

5.	Follow the procedure in [Source 3](#Source-3) below to reset to factory settings.  Then repeat the procedure to install the Soil Tester program.

#### <a id="Source-3"></a>Source 3
**Download** the original CPX **bootloader**, navigate to UF2 Bootloader Details | Adafruit Feather M0 Express | Adafruit Learning System (https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details). Scroll to the bottom of the page and click on the green rectangle, with Circuit Playground Express V#.#.# update-bootloader.uf2.  Click on the link (make sure it is for the Circuit Playground Express).  The file will download.



Click on the link (make sure it is for the Circuit Playground Express).  The file will download.

#### <a id="Program-1"></a>Program 1
To **create this program**, open makecode.adafruit.com.  Select New Project.  Add the program block code components as required below.  Save the file.  Program the CPX as listed in [Source 1](#Source-1).

<img src="/images/MakeCode_Program01.jpg" style="height: 30%; width:30%; float: left; "/>
<img src="/images/MakeCode_Program04.jpg" style="height: 30%; width:30%; float: left;"/>
<br></br><br></br>
            <br></br><br></br><br></br>
            <br></br><br></br><br></br>
    <br></br><br></br>

### Program 1 Continued

<img src="/images/MakeCode_Program06b.jpg" style="height: 30%; width:30%; float: left; "/>
   <br></br> <br></br>
            <br></br><br></br><br></br>   <br></br><br></br><br></br>
            
<img src="/images/MakeCode_Program07.jpg" style="height: 30%; width:30%; float: left;"/>
<br></br><br></br>
            <br></br><br></br>
    

Save the program by clicking on the blue Save button.  Then download the file by clicking on the pink download button.  The file will be downloaded to your download location on your computer with the same name as in the Save Box.

<img src="/images/MakeCode_Program08.jpg" style="height: 50%; width:50%; margin-left: 200px"/>


Continue with the procedure in [Source 1](#Source-1) to program the CPX with the new bootloader.
