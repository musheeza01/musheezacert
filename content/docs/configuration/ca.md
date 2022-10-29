#### Purpose
The purpose of this hands-on STEM lab is to educate students, educators, and the community about Datacenters.  Datacenters have many hundreds if not thousands of servers.  Over time parts malfunction and need repair.  Having a good inventory system is a must to track and stock inventory.  Cycle counts are performed at regular intervals to make sure the parts are ready with the datacenter technicians need it.  This activity shows how inventory cycle counts occur on a Circuit Playground Express (CPX).  The lights and actions may not exactly replicate, but loosely relate to operations at a datacenter.

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
**Prep the CPX**: Connect the USB-A/MicroUSB cable to the computer USB port.  Connect the MicroUSB end to the CPX.  Press the reset button twice, like a double-click.  A CPLAYBOOT drive should appear.  Use the information in Program 1 to add the bootloader to the CPX as in [Source 2](#Source-2).

**Power the CPX**: Insert the batteries into the battery pack.  Connect the battery pack to the CPX. Power on the battery pack

#### Go
This program contains three elements:

1.	Programming the CPX Bootloader to work with MakeCode Bootloader
2.	Using Button A and Button B to count inventory.
3.	With the switch moved to the right, Lights will display in a circular racing pattern continuously until the switch is moved to the left.
4.	While the switch is in the right position, counts are totaled by pressing Button A to add 1 and Button B to subtract 1.
5.	When the switch is moved to the left, the totals are displayed.  See [Appendix](#Appendix) for details.
6.	Moving the switch back to the right position will reset the counts and restart the program.

See [Appendix](#Appendix) for Details. Use the [Lesson](#Lesson) information to explain the lab to relatable concepts at the Datacenter.

#### After
Note any items that are damaged, not working, or missing (including consumables) as noted in Get Help below.

#### Source
1.	The program utilizes a simple code in MakeCode. See [Program 1](#Program-1) below for programming details.

#### Get Help
For any questions contact the Microsoft Datacenter Community Development team at dc-stem@microsoft.com

#### <a id="Appendix"></a>Appendix
Cycle counts are a normal regularly scheduled process for each Inventory and Asset Technician.  Accurate counting allows for parts to be ordered and available when needed for repairs.  To begin this program, verify the switch is on the right.  Connect the battery adapter.  The lights should race around the Circuit Playground Express in a rainbow pattern.  If the CPX does not light, move the switch to the left and then to the right to restart the program.

While the lights are racing and the switch is to the right, press Buttons A and B to add or subtract from the count.  When cycle counts are complete, move the switch to the left.  The Circuit Playground Express will display the counts as follows:

Blue will display the Tens value

<img style={{ clear: "right", float: "left", height:"300px", width:"300px"}}
            src="/images/blueten.png" />


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
<br></br>

Green will display the Ones Value	

<img style={{ clear: "left", float: "left", height:"300px", width:"300px"}}
            src="/images/greenten.png" />


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
<br></br>

To run the Inventory In/Out program, press Button A.  The lights will race around the CPX in a rainbow of colors for 2 seconds.  Then, the selection will be made at random.  One of three choices will be selected, signified by the example images below:

1. The part is not in inventory. Check with the Inventory and Asset Technician for stock information.
2. The part is in inventory.  Scan the part out for your repair.
3. Scan the part back into inventory.

<img style={{margin:"0px", clear: "left", float: "left", height:"400px", width:"300px"}}
            src="/images/circuitcolors.png" />
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
<br></br>

Red will display a Zero or Negative count
The lights will blink and a siren will be heard.

<img style={{margin: "0", clear: "left", float: "left", height:"400px", width:"300px"}}
            src="/images/redten.png" />

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
<br></br>

Circle lights indicate double digits for the cycle counts.

<img style={{margin:"0px 0px 0px 0px", clear: "left", float: "left", height:"400px", width:"300px"}}
            src="/images/purpleten.png" />

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
<br></br>

#### <a id="Lesson"></a>Lesson
Datacenters have many hundreds if not thousands of servers.  Over time parts malfunction and need repair.  Having a good inventory system is a must to track and stock inventory.  Cycle counts are performed at regular intervals to make sure the parts are ready with the datacenter technicians need it.  This activity shows how inventory cycle counts occur on a Circuit Playground Express (CPX).  The lights and actions may not exactly replicate, but loosely relate to operations at a datacenter.

#### What:
This lab demonstrates datacenter inventory protocols and demonstrates cycle counting parts in inventory.  

#### Details:
Inventory and Asset Technicians keep the Microsoft Cloud running by assuring the correct parts are in stock in inventory.  Cycle counts allow Datacenter Technicians to quickly find parts needed for repair.  Counting the parts at regular intervals provides data needed to order new parts.  When parts are out of stock, the Inventory and Asset Technicians will order new stock during their routine cycle counts.  During this count, the Inventory and Asset Technician may find parts incorrectly placed in inventory.  This is corrected as the part is moved to the correct location and the inventory count corrected.

#### Share:
Defining the Cloud, servers, and common server parts may be helpful prior to explaining the lesson.  The datacenter is a building full of servers.  Servers are different than computers in your lab or classroom as they do not have a monitor or keyboard but do have many disks.  The disks contain data.  Data can be account information for banking or online shopping, medical lab tests, schoolwork, video game accounts, photos, or email.  When a server has a problem, technicians work fast to replace the parts promptly to keep the cloud running.

NOTE:
This lab works by pressing Button A to add to the count and Button B to subtract from the count.  Moving the switch to the left will display the count.  See the [Appendix](#Appendix) for more information on the values.  Moving the switch to the right will reset the count and allow the next cycle count to occur.

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
1.	Check the batteries
2.	Press reset button 1 time.  This will reset the device, like a computer reboot/restart.
3.	Follow steps in Source 1 to download the program to the CPX device.
4.	Try another device and see if the problem repeats.  If it repeats check program in Source 1 and 2 to install the program again.
5.	Follow the procedure in [Source 3](#Source-3) below to reset to factory settings.  Then repeat the procedure to install the Intrusion program.

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
To **create this program**, open [MakeCode.adafruit.com.](MakeCode.adafruit.com.) Create the bootloader file by creating the block code program below:

Program the CPX as listed in [Source 1](#Source-1). with the code below.

<img style={{margin: "0", clear: "left", float: "left"}}
            src="/images/circuitplaygroundcount.png" />
            
