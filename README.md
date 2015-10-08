# Kamloops Makerspace UP! Printer Documentation

Kamloops Makerspace 3d printer is heavily modified version of UP! from PP3DP company.
Controller motherboard was replaced with [Smoothieboard](http://smoothieware.org/smoothieboard).

Power supply is 20V 30A. There are two separate voltage regulator devices mounted inside the enclosure: one for 5V with 2x USB sockets and one for 12V line.

12V line powers two fans: one for PLA cooling and one inside the enclosure for cooling the electronics. 12V line also powers the LED strip.

Raspberry Pi is hidden inside the printer enclosure. It is powered by 5V regulator device.
Services that are running on the pi: ssh-daemon, octoprint (port 80 through haproxy). Administrator login to ssh is pi:pi, to octoprint is admin:admin.

# UP! 3D Printer to Smoothieboard conversion

## Specifications

### Motors
* Set current limit to 0.4 amp
* alpha (x)
* beta (y)
* gama (z)
* delta (extruder)
 * blue+green and yellow+orange wires

### Extruder
 * Wires are doubled up: yellow+orange and blue+green
 * Extruder fan: black and white wires
 * Thermistor is 110 ohm at 23 degree celcius
 * Thermistor on purple and gray wires

### Heated bed
 * Thermistor resistance:
 * Thermistor wires:

### Limit switches
There are 3 optical limit switches on the UP printer, one for each axis.
