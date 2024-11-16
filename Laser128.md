# Laser 128 Support
TangyPack now works (using Firmware V1.10) on the Laser 128, with a few caveats.    <br/>Tangy Pack will auto detect when plugged into the Laser 128.

* **The original case that shipped with the Tangy Pack will not fit on the Laser 128.  Laser 128 compatible case stl is available in the Case STL folder if you have a 3D printer and you want to print your own.  Tangy Pack purchased on/after November 2024 will come with the Laser 128 compatible case**
* The case and firmware was tested with the newer style Laser 128 with  Rom V4.3 and V6.0 <br/> I do not have the old style laser 128, Laser 128EX or EX/2 so untested on these machine.  If you have these machine and the Tangy Pack works on it, please drop me a note.
* Laser 128 must have the MONO/COLOR switch in MONO setting. (Tangy Pack will display color images)
* Tangy Pack is not using the RGB signals on the Laser 128. It is using the digital serial output data and displaying the image in same way it does with the Apple IIc.  
* Laser 128 is missing the GR signal available on the Apple IIc that is used to kill the color on text modes.  This means, the Laser 128 display will always display in color unless you change the mode on the Tangy Pack itself using the "B" button.
* CREF (color reference) signal available on the Apple IIc is missing from the Laser 128.  I am internally generating the color reference from the sync video signal. Unfortunately, the color reference has different timing relationship in double high res mode and I can not detect this. <br/> So, button "A", when in Laser 128 mode, allows you to manually change the internal CREF state.  There are four valid CREF state. Each press of the button A changes the mode in the following order.
  * CREF state A - Scan line on (Default)
  * CREF state A - Scanline off
  * CREF state B - Scanline on
  * CREF state B - Scanline off
  * CREF state C - Scan line on
  * CREF state C - Scanline off
  * CREF state D - Scanline on
  * CREF state D - Scanline off
* The video timing is just a tad more out of spec compare to the Apple IIc after scan doubling.  This means some finicky monitors that work with the Tang Pack in the Apple IIc mode will not work on the Laser 128.