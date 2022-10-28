# CPX Circuit On/Off
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
Read through [Source 1](#Source-1) below.  When you are ready, move the image ([Source 2](#Source-2)) to the CPX.  Use instructions located here: [Source 2](#Source-2).  Test the program.

#### Get Ready
**Prep the CPX**: Connect the USB-A/MicroUSB cable to the computer USB port.  Connect the MicroUSB end to the CPX.  Press the reset button twice, like a double-click.  A CPLAYBOOT drive should appear.  Use the information in [Program 1](#Program-1) to add the bootloader to the CPX as in [Source 2](#Source-2).


**Power the CPX**: Insert the batteries into the battery pack.  Connect the battery pack to the CPX. Power on the battery pack.

#### Go
This program contains three elements:
1. Programming the CPX Bootloader to work with MakeCode Bootloader
2. Using Button A to randomly select inventory status on a part.
3. Lights will display in a circular racing pattern for 2 seconds, then randomly select 1/3 of the lights.
4. Using the [template](#template) to define the selection of the randomly displayed lights will determine the inventory status outcome.

See  [Appendix](#Appendix) for Details. Use the [Lesson](#Lesson) information to explain the lab to relatable concepts at the Datacenter.

#### After
Note any items that are damaged, not working, or missing (including consumables) as noted in Get Help below.

#### Source
1. The program utilizes a simple code in MakeCode.  See [Program 1] (#Program-1)below for programming details.

#### Get Help
For any questions contact the Microsoft Datacenter Community Development team at dc-stem@microsoft.com

#### <a id="Appendix"></a>Appendix
Print the Template and place the Circuit Playground Express (CPX) in the center dotted circle.  Connect the battery pack with the battery adapter port (black) down.  The cables connected between the CPX and the battery adapter should follow the center line on the bottom half of the circle. Once connected, the lights will be off except for a small green led associated with the On sensor.
<img style={{ clear: "right", float: "left", height:"400px", width:"300px"}}
            src="/images/inventory.png" />

<br></br>
<br></br><br></br>
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

To run the Inventory In/Out program, press Button A.  The lights will race around the CPX in a rainbow of colors for 2 seconds.  Then, the selection will be made at random.  One of three choices will be selected, signified by the example images below:

1. The part is not in inventory. Check with the Inventory and Asset Technician for stock information.
2. The part is in inventory.  Scan the part out for your repair.
3. Scan the part back into inventory.

<img style={{margin:"0px", clear: "left", float: "left", height:"400px", width:"300px"}}
            src="/images/circuitcolors.png" />

<img style={{margin:"0px 0px 0px 50px", clear: "right", float: "left", height:"400px", width:"300px"}}
            src="/images/circuitred.png" />

<br></br>
<br></br>
<br></br><br></br>
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
<img style={{margin: "0", clear: "left", float: "left", height:"400px", width:"300px"}}
            src="/images/circuitblue.png" />

<img style={{margin:"0px 0px 0px 50px", clear: "right", float: "left", height:"400px", width:"300px"}}
            src="/images/circuitgreen.png" />

<br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br>
<br></br>

#### <a id="Lesson"></a>Lesson
The purpose of this hands-on STEM lab is to educate the community about Datacenters.  The lights and actions may not exactly replicate, but loosely relate to operations at a datacenter.

#### What:
This lab demonstrates datacenter inventory protocols and demonstrates checking out or returning a part to stock..  

#### Details:
Inventory and Asset Technicians keep the Microsoft Cloud running by assuring the correct parts are in stock in inventory.  Sometimes parts are removed and not needed.  This could be because it wasn’t the correct part or did not resolve the problem.  Datacenter Technicians will return the part to inventory, so it is ready for the next repair.  When parts are out of stock, the Inventory and Asset Technicians will order new stock during their routine cycle counts.

#### Share:
Defining the Cloud, servers, and common server parts may be helpful prior to explaining the lesson.  The datacenter is a building full of servers.  Servers are different than computers in your lab or classroom as they do not have a monitor or keyboard but do have many disks.  The disks contain data.  Data can be account information for banking or online shopping, medical lab tests, schoolwork, video game accounts, photos, or email.  When a server has a problem, technicians work fast to replace the parts promptly to keep the cloud running.

NOTE:
This lab works by pressing Button A, then a random selection is made.  The illuminated section of the CPX board defines the inventory status from the template.  This cycle can be repeated to demonstrate how inventory may or may not be available for repair.

#### <a id="Source-1"></a> Source 1 
The Adafruit Circuit Playground Express (CPX) is a microcontroller with more power, storage space, and RAM than a 386 Intel Computer.  It includes temperature, light, sound, and accelerometer sensors, 10 built in LEDS, speaker, two push buttons, one slide switch, IR receiver and transmitter, 8 analog inputs, power output, 7 capacitive touch inputs, green "ON" LED, reset button, ATSAMD21 ARM Cortex M0 Processor, 2 MB of SPI Flash storage, and a Micro USB port for programming and debugging.

Source:
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

Copy the saved UF2 file from the Intrusion folder and paste it on the CPLAYBOOT root drive.

The CPX lights will flash, then reset and the CPLAYBOOT drive will disappear from the drive list.

The program is now installed

Press the reset button on the CPX.

Once the Circuit Playground Express (CPX) is connected, without MiniGrabbers attached, all LEDs will display blue. 

To **troubleshoot** the CPX device and program:

1. Check the batteries
2. Press reset button 1 time.  This will reset the device, like a computer reboot/restart.
3. Follow steps in Source 1 to download the program to the CPX device.
4. Try another device and see if the problem repeats.  If it repeats check program in Source 1 and 2 to install the program again.
5. Follow the procedure in [Source 3](#Source-3) below to reset to factory settings.  Then repeat the procedure to install the Intrusion program.

#### <a id="Source-3"></a>Source 3
**Download** the original CPX **bootloader**, navigate to [UF2 Bootloader Details | Adafruit Feather M0 Express | Adafruit Learning System](https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details) (https://learn.adafruit.com/adafruit-feather-m0-express-designed-for-circuit-python-circuitpython/uf2-bootloader-details). Scroll to the bottom of the page and click on the green rectangle, with Circuit Playground Express V#.#.# update-bootloader.uf2.  Click on the link (make sure it is for the Circuit Playground Express).  The file will download.

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
To **create this program**, open [makecode.adafruit.com.](MakeCode.adafruit.com.) Create the bootloader file by creating the block code program below:

<img style={{margin: "0", clear: "left", float: "left", width: "300px"}}
            src="/images/animation.png" />
            <br></br><br></br>
<br></br><br></br>
<br></br><br></br>
<br></br><br></br>
<br></br><br></br>
<p style={{margin: "20px 0px 0px 340px"}}>Program the CPX as listed in [Source 1](#Source-1).</p>
<br></br><br></br>
<br></br><br></br>
            
<img style={{margin: "0",  clear: "left", float:"left", height:"300px", width: "300px"}}
            src="/images/elseif.png" />
<br></br><br></br>
<br></br><br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>

### <a id="template"></a> Template
Use the following template for the CPX and this program.  Place the CPX board in the center of the dotted circle with the battery adapter port facing towards the bottom of the page along the center line as noted in the diagram.

<img style={{margin: "0px 0px 0px 50px", clear: "left", float: "left", width: "300px"}}
            src="/images/template.png" />
