# TouchOSC layout for 24 channels (1 mixer strip)

This layout is influenced by the original 24channel-1fader-tab.

* It is designed for modern Android tablets, having 16:10 screens 
  (e.g. 1280x800)
* It includes a master slider.

Fun fact: This layout is not designed with the TouchOSC layout editor,
but programmatically generated.

[Screenshot](24channel-1fader-alt-tab.png)

Included is a preset file for Ardour5. Just put it in your
`~/.config/ardour5/osc/` directory and restart Ardour. You can choose
the preset from the OSC settings dialog. **Note** the preset uses
remote port 8000, you may need to change this if you have configured
TouchOSC to use a different port.

# Instructions

* Turn on OSC in Ardour in Perferences > ControlSurfaces.
* Open the settings GUI.
* Either select the "24 Channels, no master" preset or:
* Set Port Mode to Manual, port 8000 is fine.
* Set Bank Size to 24.
* Set Gain Mode to Position.
* In the Default Strip Types tab: check the top six lines for a Strip
  Types Value of 159.

Install TouchOSC on your tablet if it is not already installed.
Run/open TouchOSC:

* Set the IP address to the IP of the computer running Ardour.
* Set the send port to 3819, or whatever you've configured in Ardour.
* Set the receive port to 8000, or whatever you've configured in Ardour.
* Download the accompanying file to your tablet and find it with
  touchOSC and load it. 

The layout should display horizontally. Depending on your TouchOSC
settings it may be upside down. Complaints to
https://facebook.com/touchosc .

In the bottom left corner touch the 'Connect' button.

The first up to 24 track names should appear. Busses and master are
not shown. The LEDs around the track buttons, starting
from top and clockwise: signal (green), monitor input (orange),
monitor disk (brown), solo (green), mute (yellow), record safe
(green), record enable (red).

# Issues

Please send issues to the Github issue tracker.

# License

This is free software. Use it for watever purposes you like.

Copyright 2019, Johan Vromans
