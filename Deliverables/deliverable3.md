# Deliverable 3

For this week's deliverable, you'll be testing some of the functionality of your Raspberry Pi and additional hardware by using the DFRobot LCD Hat, the KY40 Rotary Encoders, and accessing it's GPIO. You'll also be creating an initial circuit diagram for your system.

## Verify Hardware (P)

Before or during class on Friday, you must return the hardware listed in [Deliverable 2](deliverable2.md) by either going to Dr.Herring's (Driftmier 1202) or Dr.Trudgen's (Driftmier 1200) Offices throughout the week or by showing up to class.

## Wiggle Motors (D)

First, you'll need to demonstrate that you can take advantage of some of the basic features of the DFRobot LCD necessary for creating a useful user interface. Before attempting to use the LCD, make sure the Adafruit motor hat is either off of the Pi, or its `I2C` address has been changed by creating a solder bridge on the `A0` jumper, otherwise the LCD will not be able to communicate with the Pi.  This is clearly described in Deliverable 4.  For now don't have the Motorhat and the DFRobot LCD both on the PI at the same time.

**P**: To demonstrate grasp of how to set up and use the LCD and its buttons, create a program which displays an integer starting at 0 on the LCD. Whenever the top LCD button is pressed, the number increments by 1 and whenever the bottom LCD button is pressed, the number decrements by 1.

To accomplish this, you'll need to read through the [DFRobot LCD documentation](https://wiki.dfrobot.com/I_O_Expansion_HAT_for_Pi_zero_V1_0_SKU_DFR0604IIC_16X2_RGB_LCD_KeyPad_HAT_1_0_SKU_DFR0514_DFR0603). We've included the library needed to use the LCD (`rgb1602.py`) under the `lib` directory in your starter repository on the class Github, and you should look through it to get an idea of how to use the LCD. It should also be helpful to look through the [DFRobot provided examples on Github](https://github.com/DFRobot/DFRobot_RGB1602_RaspberryPi).

## Characterize Microphone(P)

To provide user input to the plotter, two rotary encoders will be used. To simplify the development of this project for you, you will be using the [Pigpio Encoder Python library](https://github.com/vash3d/pigpio_encoder)

The library should already be included in your group repository, under the `lib` directory.

The Github page gives a through explanation of how to use the library. 

**P**: To demonstrate a basic understanding of how to use the KY40 Rotary Encoder, create a program which increments and prints an integer on the LCD when you turn the encoder to the right, and decrements and prints the integer on the LCD when you turn the encoder to the left.

> Pitfall: If you install the pigpio encoder library with pip, ie pip install pigpio_encoder, it will install an older version of the library that does not include some of the functions like up_callback()
and down_callback().

## Accessing and Using A GPIO (P)

>***Warning: while connecting up simple components to the GPIO pins is perfectly safe, it's important to be careful how you wire things up. LEDs should have resistors to limit the current passing through them. Do not use 5V for 3V3 components. Do not connect motors directly to the GPIO pins, instead use an H-bridge circuit or a motor controller board.***

Next, you'll need to demonstrate that you can access and use a GPIO as both input and output. Your Raspberry Pi should have come with a breadboard, some jumper wires, and some resistors, LEDs, and buttons for this deliverable.

**P**: To demonstrate output, create a Python script to blink an LED, either with user control or on a set interval. To demonstrate input, use the guides below to create a Python script to print a statement once on the screen whenever a button in the real world is pressed.

For both of these you'll need to use the [`pigpio` Python library](http://abyz.me.uk/rpi/pigpio/index.html#Type_3), with its API [Reference](http://abyz.me.uk/rpi/pigpio/python.html) and some [example code](http://abyz.me.uk/rpi/pigpio/examples.html#Python%20code). Again, make sure to use a current-limiting resistor when using the GPIO as output, and enable the [Pull-Up or Pull-Down](https://en.wikipedia.org/wiki/Pull-up_resistor) feature on the pin when using it as input. (Note: Make sure to use the `pinout` command in a terminal to check wiring and pin numbers).

### Tips on using Using GPIO as input

While you're creating your GPIO input script, you'll notice that a simple polling method of using the GPIO may not give the results desired. To remedy this, we suggesting looking into setting up [interrupts/callbacks](http://abyz.me.uk/rpi/pigpio/python.html#callback) with the GPIO pins, or using [software debounce](https://www.arduino.cc/en/Tutorial/BuiltInExamples/Debounce).



# Summary

In summary, for this week you need to:

1. Make sure you have returned the unused hardware listed in [Deliverable 2](deliverable2.md) to Dr.Herring or Dr.Trudgen either before or during class on Friday. You can return then to Dr.Herring's (Driftmier 1202) and Dr.Trudgen's (Driftmier 1200) Offices throughout the week or in class on Friday.

2. Submit evidence in the form of pictures/videos for your **P** deliverable items to the Progress Deliverable 3 assignment folder on ELC. You do not need to submit code on ELC, just make sure your GitHub repository is up to date and contains the needed scripts.  Make sure videos are short (less than 30 seconds per video), clear, and are narrated so that you communicate what you are showing.  Do not sumbit Apple only playable videos or photos.  They should be playable by standard software readily available. If you submit photos, make sure that they are labeled or identify in some way what you are showing.

2. Bring your wiring diagram for the Adafruit Motor Hat pins to the new stepper motor wiring (Use colors of wires to the pins).  We will check this in class on Friday and provide you your new stepper motors.

3. Submit your completed Circuit Diagram to the Design Deliverable 3 assignment folder on ELC.

4. Update your User Manual and Technical Documentation with your findings.

5. Submit your Weekly Project Management Report to the "WPM for Deliverable 3" assignment folder on ELC.
