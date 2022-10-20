# CPX Bruno music, IR Tag, and DC Light Signals
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
**Prep the CPX** : Connect the USB-A/MicroUSB cable to the computer USB port.  Connect the MicroUSB end to the CPX.  Press the reset button twice, like a double-click.  A CPLAYBOOT drive should appear.  Use the information in Program 1 to add the bootloader to the CPX as in [Source 2](#Source-2). 

**Power the CPX**: Insert the batteries into the battery pack.  Connect the battery pack to the CPX. Power on the battery pack.

#### Go
This program contains three elements:

1.	Plays the tune 'Bruno' from the movie Encanto (Switch moved to left)

2.	IR Tag 'laser' transmitted (Button B)

3.	Reset lights, tag count, and cycles signal lights red/yellow/blue (Button A)

See  [Appendix](#Appendix) for Details. Use the [Lesson](#Lesson) information to explain the lab to relatable concepts at the Datacenter.

### After
Note any items that are damaged, not working, or missing (including consumables) as noted in Get Help below.

### Source
1.	IR Tag, Reset, and 'Bruno' from Encanto are all programmed through Makecode.adafruit.com. See [Program 1](#Program-1) below for programming details.

### Get Help
For any questions contact the Microsoft Datacenter Community Development team at dc-stem@microsoft.com

#### <a id="Appendix"></a>Appendix

<p> The TrioCombo program is ready and  </p>

<p style={{ margin: " -50px 0px 0px 400px" }}> Moving the switch to the left will play the tune 'Bruno'</p>

<p style={{ margin: " -35px 0px 0px 000px" }}>installed when all lights display blue.</p>
                           
<p style={{ margin: "08px 0px 0px 400px" }}> from the movie Encanto</p>

<p style={{ margin: "08px 0px 0px 400px" }}> Lights will change in color after each note.</p>

<br></br>

<img style={{ margin: "0px", clear: "right", float: "left", height:"300px", width: "300px" }}
            src="/images/skybluelights.png"
            /> 
<img style={{ margin: "0px", clear: "right", float: "right", height: "300px", width: "300px" }}
            src="/images/magentalights.jpg"
            />

<br></br><br></br>
<br></br><br></br>
<br></br><br></br>
<br></br><br></br>
<br></br><br></br>
<br></br><br></br>

Pressing the A button (left button when battery adapter is facing down) will cycle signal lights from green, yellow, red.  Then the lights will reset at blue.  This also resets the IR tag count.

<img style={{ margin: "0px", clear: "right", float: "left", height: "300px", width: "300px"}}
            src="/images/greenir.png"
            /> 
<img style={{ margin: "0px", clear: "right", float: "left", height: "300px", width: "300px"}}
            src="/images/redir.png"
            /> 
<img style={{ margin: "0px", clear: "right", float: "left", height: "300px", width: "300px"}}
            src="/images/yellowir.png"
            /> 


<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br><br></br><br></br>

IR Tag is played by pressing the B button to transmit (TX) the signal to an opposing CPX where the signal will be received (RX).  The ‘pew-pew’ sound is heard when the button is pressed (think Atari Asteroid game).  The dying sound is heard when the IR signal is received by the opposing device (think Atari and last life).  Blue lights indicate not yet hit/tagged or game reset.  Red lights indicate hit/tagged .

