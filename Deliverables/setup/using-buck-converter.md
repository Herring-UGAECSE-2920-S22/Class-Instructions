# Using the Buck Converter

Your buck converters can output 3A from 1.25V - 30V. Test this voltge

From the picture below, you'll want to put some jumper pins onto the Input+/- and Output+/- as directly soldering wires onto a board like this could cause issues in the future. After that, connect leads from your 12V power supply to the Input+/- pin and connect a voltmeter (or multimeter in voltage mode) to the Output+/- pins. With your 12V power supply on, adjust the output voltage to 5V by turning the voltage adjustment screw on the module clockwise to increase the output voltage and counter-clockwise to decrease the output voltage.

<img width="695" alt="Screen Shot 2022-01-21 at 3 06 48 PM" src="https://user-images.githubusercontent.com/49916015/150593329-5dcf954d-5d4f-4a45-a9ff-962ca3e85e52.png">


When you have adjusted the module to output 5V, you can then use it in place of your linear regulator for your H-Bridge circuit.
