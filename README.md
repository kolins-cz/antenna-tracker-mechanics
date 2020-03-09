# antenna-tracker-mechanics
##  Antenna tracker mechanics with stepper motors made specifically for Open.HD project
This is supposed to be ultimate antenna tracker for heavy antennas superior to any existing and future RC-servo based design.

Stepper motors do not jitter / oscillate when subjected to static torque. This is common problem for RC-servo based trackers especially on TILT axis. This tracker will hold position without any movement. With proper control software, movement can be really smooth.

Tracker is designed with a slip ring on PAN axis. This allows non-rotating control electronics and indefinite rotation of PAN axis. 
For Open.HD use, USB shall be routed through slipring from Ground Pi housed in lower static part to upper rotating part. TILT Stepper motor is also powered trough slipring.


##  Done
* Tilt Axis Assembly
* Movement tests with control board for 3D printers

##  Work in progress but tested
* Pan Axis Assembly

##  Work in progress but untested
* Tripod mounting assembly
* Lower part for housing electronics (this will probably change several times)

##  Future
* Software / Firmware support

##  Components
* 3D printed parts, easy
* 8mm hollow tube. Hope USA users can get this. Very common in hardware stores in Europe. Needs to be cut to length with hack saw
* M3 screw rod cut to correct length
* M3 nuts
* Various wood screws
* 4x 608 Bearing
* 4x M3 60mm metal stand-offs 
* 1x 1/4-20 UNC nut for tripod mount
* 1x Strong 46mm x 60mm x 1.6mm plate for tripod mount. Can be old PCB, Aluminum, FR4, G10, CF etc... Needs to be hand cut and drilled unless you have CNC 



##  FAQ
Q: Can I build one?
A: Sure you can! Download .step file take a look. It is not finished and things may change. 

Q: Where are the .stl files?
A: There will be none until project is finished. Right now, you will need some CAD knowledge

Q: I can’t source component X. What can I do?
A: Download .step file and make necessary changes in your favorite CAD software (something like Fusion 360)

Q: Is there ready firmware solution to work with this?
A: No. For tests I use old RAMPS board with Marlin firmware inside. It can accept G code and make the tracker moving. Config.h for marlin is available for download

Q: How can I contribute?
A1: Probably by pull request via github with modified .step file. I will download one and take a look and merge changes.
A2: Code support for this. There are nice antenna tracker firmware projects around but none has support for stepper drivers. Most notorious are probably Ghettostaion, uu360gts, zs6buj tracker, Ardutracker and so on. Pick one

Q: Licence?
A: GNU GPL v2.0
