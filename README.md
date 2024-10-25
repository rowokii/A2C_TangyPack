# A2C_TangyPack
Allows VGA and HDMI (DVI) video device to be connected to Apple IIc/IIc+ (US NTSC Machine only). 

If you want to purchase one, it's avaiable from ct6502.org: [https://ct6502.org/product/tangypack/](https://ct6502.org/product/tangypack/)

### WARNING!!!  Do not plug/unplug the device to/from the Apple IIc with the power on.  Damage to the device and/or to your Apple IIc can occur.  It is strongly recommended to lock the screw terminal down to prevent the device from being accidentally disconnected. 

* HDMI specification allows for hot plugging the connector.  
* Hot plugging VGA connector is not defined in the specification and there is mixed information regarding if it is safe.


# Descrpition
A2C_TangyPack plugs into the video expansion port of the Apple IIc/IIc+ and is powered from the port itself.  It is a scan doubling device that will take the 560x192 video of the Apple IIc and upscale the video to ~640x480 (720x480 @ 28.63MHz pixel rate) video resolution supported by most modern video monitors. 

## Compatibility Warning

### Tangy Pack supports only US NTSC machines.
### Not recommended for HDMI Video Capture devices at this time.  It looks like most HDMI Video Capture devices does not support 640x480 resolution

Some monitors have problems detecting or auto sizing the image since the video from the Apple IIc is smaller than normal 640x480 image.  Turning on the border can help the monitor detect and lock on to the video.

After testing with different type of video devices, it seems like some wide screen TVs and video capture cards has problems detecting the video from this device, even with the border turned on.  This is mainly on the hdmi output.  

Also, please be aware some displays will scale and apply image filtering to the input images which will destroy the scanline effects and/or stretch the image from it's normal 4:3 size.

This device currently does not work with IIc+ that has been accelerated to run faster than the stock IIc+.

## Controls
Controls are simple.  Push the corresponding buttons to cycle through the options listed. Power on defaults are the first options of each row.  
  
  A - Toggles scanline effect On/Off  
  B - Color mode, Mono Green, Mono Amber, Mono White  
  C - Border off, Border White, Border Blue, Border Green  
  
![Front_View](./Images/front_view_buttons.jpg)

# Firmware
Currently there is only one firmware available for the Tangy Pack.  (See Firmware folder)  

However, there is a firmware update mechanism in place for any future firmware release. 

[Firmware Update](./Firmware/Firmware.md)
