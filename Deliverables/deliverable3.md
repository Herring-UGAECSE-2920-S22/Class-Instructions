# Deliverable 3

For this week's deliverable, you'll be testing some of the functionality of your Raspberry Pi and additional hardware by using the DFRobot LCD Hat, the KY40 Rotary Encoders, and accessing it's GPIO. You'll also be creating an initial circuit diagram for your system.

## Verify Hardware (D)

Using your [hardware list](./images/PartList.jpg) check all the parts in your kit and make sure you not only have them but they are in working condition this will be important as you begin your project and at the end when you return the kits. Please turn in a filled our status sheet for your parts.

## Wiggle Motors (D)

First, you'll need to demonstrate that you can take advantage of some of the basic motor features necessary for creating a functional audio car. This means getting your motors to move. So create a program demonstrating both motors moving and also one motor moving at a time.

**Hint**: Take a look at [python multithreading](https://realpython.com/intro-to-python-threading/) in order to protect your program as you run methods for both motors.

To accomplish this you willl need to know how to **access and use a GPIO:**

>***Warning: while connecting up simple components to the GPIO pins is perfectly safe, it's important to be careful how you wire things up. LEDs should have resistors to limit the current passing through them. Do not use 5V for 3V3 components. Do not connect motors directly to the GPIO pins, instead use an H-bridge circuit.***

Next, you'll need to be able to access and use a GPIO as both input and output. Your Raspberry Pi should have come with a breadboard, some jumper wires, and some resistors, LEDs, and a DIP Switch. In order to test your ability to use a GPIO as an input and output create a Python script to blink an LED, either with user control or on a set interval. To demonstrate input, use the guides below to create a Python script to print a statement once on the screen whenever the DIP Switch is on in the real world.

## Characterize Microphone(D)


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

1. **D**: Make sure all your hardware is in your kit and is in working shapes and fill out the parts checklist

2. **D**: Wiggle your DC Motors(forward, backward, and one by one).

3. **D**: Characterise your Microphone. See how sensitive it is and make sure it is characterized enough to do what you need it to with your Audio Car.

4. Update your User Manual and Technical Documentation with your findings.
