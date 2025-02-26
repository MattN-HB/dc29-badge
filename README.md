# dc29-badge

## Firmware
To get started, please update your firmware.

* Step 1: You will need to download new firmware for your badge to participate, this firmware can be found here https://defcon.org/signal/ (this link can be found in the topic of #dc29-badge as well if you don't trust me).
* Step 2: Connect your badge to your PC with usb-c on badge side, and usb-a on computer. Turn power switch from battery to USB while holding down the bottom right button, your badge should glow red.
* Step 3: You should see your badge as an attached USB drive. Drag and drop the new firmware into your badge. It should automatically reboot.

## Connecting from computer

* *macOS*, you can run `screen /dev/tty.usbmodem123451 9600` which will present a black screen, then press enter. 
* *linux*, you can run `Sudo screen /dev/ttyACM0 6900-8-D-1` or `Minicom --device /dev/ttyACM0`. NOTE: you may need to find the right TTY device, it may be named something other than usbmodem123451.  Use ```Dmesg | grep tty``` to find. also important to know that toggling battery usb will bring serial up.
* *Windows* use your favorite terminal (Putty/Mobaxterm/etc.), new Serial session, COM3 (maybe COM4 etc.) and typically 9600 speed, then you should see a black screen, press enter.

## Simon says

To play Simon says, 

* Simon says to power on your badge while holding the top-left button

## Connecting / Pairing / Interfacing

```
Number of Badges Connected: 25
Badge Types Collected: Human,Goon,Creator,Speaker,
```

To connect to another badge you have two options, physically and digitally.

### Physically
Connect the wide port on the side of the badge to another's port while both are powered on in the normal mode (non-simon, non-flash).

### Digitally
When connected to the terminal of the badge, you can generate requests for others to connect to YOU. Press '4' to generate the request and press '5' to enter the other badge's response. You will then want to ask for someone elses request. Press '5' to enter their request, and then send them the generated response.

## Debugging

Known issues:

1. Some badges are known to output invalid codes, usually [31 chars long instead of expected 32](https://github.com/d1str0/dc29-badge/issues/1). No known fix.

## Pro-Tips

1. Remap one of your keys to output your request code.
2. Remap a key to your personal github to land a new job!

## Resources/Fav Talks
* [Signal DC](https://defcon.org/signal/instructions.html)
* [All Docs at Info on](https://infocon.org/)
* [Cloud village](https://cloud-village.org/)
* [Iot village](https://www.iotvillage.org/defcon.html)
* [Aerospace village](https://m.youtube.com/c/AerospaceVillage)
* [Wall of sheep](https://www.youtube.com/wallofsheep)
* [Adversary village](https://m.youtube.com/channel/UCOhn9WALnpb5YAbW18R1Hzg)
* [DEFCON YouTube](https://m.youtube.com/user/DEFCONConference)
* [Badge hackaday](https://hackaday.com/2021/08/05/hands-on-def-con-29-badge-embraces-the-new-normal/)
* [Carhacking keynote by Allisa Knight](https://youtu.be/X0ZNEyzloY8)
* [Media server all talks and docs](https://dc29-media.defcon.org) `wget -np -m https://dc29-media.defcon.org/infocon.org/cons/Def Con/DEF CON 25/`
* [Infocon](https://infocon.org/cons/DEF%20CON/DEF%20CON%2029/)
