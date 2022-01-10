# Deliverable 3

For this week's deliverable, you'll be testing some of the functionality of your Raspberry Pi and additional hardware. You'll also be using that hardware to get your motors moving and you microphone characterized.

## Verify Hardware (D)

As a continuation from last week, using your [hardware list](./images/PartList.jpg) check all the parts in your kit and make sure you not only have them but they are in working condition this will be important as you begin your project and at the end when you return the kits. Please turn in a filled our status sheet for your parts.


## Accessing and Using A GPIO 

>***Warning: while connecting up simple components to the GPIO pins is perfectly safe, it's important to be careful how you wire things up. LEDs should have resistors to limit the current passing through them. Do not use 5V for 3V3 components. Do not connect motors directly to the GPIO pins, instead use an H-bridge circuit or a motor controller board.***

As you begin to use your Raspberry Pi to work your motors, you'll need to demonstrate that you can access and use a GPIO as both input and output. Your Raspberry Pi should have come with a breadboard, some jumper wires, and some resistors, LEDs, and a DIP switch for this demonstration.

**Practice:** To demonstrate output, create a Python script to blink an LED, either with user control or on a set interval. To demonstrate input, use the guides below to create a Python script to print a statement once on the screen whenever the switch is flipped in the real world.

For both of these you'll need to use the [`pigpio` Python library](http://abyz.me.uk/rpi/pigpio/index.html#Type_3), with its API [Reference](http://abyz.me.uk/rpi/pigpio/python.html) and some [example code](http://abyz.me.uk/rpi/pigpio/examples.html#Python%20code). Again, make sure to use a current-limiting resistor when using the GPIO as output, and enable the [Pull-Up or Pull-Down](https://en.wikipedia.org/wiki/Pull-up_resistor) feature on the pin when using it as input. (Note: Make sure to use the `pinout` command in a terminal to check wiring and pin numbers).

### Tips on using Using GPIO as input

While you're creating your GPIO input script, you'll notice that a simple polling method of using the GPIO may not give the results desired. To remedy this, we suggesting looking into setting up [interrupts/callbacks](http://abyz.me.uk/rpi/pigpio/python.html#callback) with the GPIO pins, or using [software debounce](https://www.arduino.cc/en/Tutorial/BuiltInExamples/Debounce).


## Wiggle Motors (D)

Now that you know how to use your raspberry pi's GPIOs you now can use them to move your motors.

First, you'll need to demonstrate that you can take advantage of some of the basic motor features necessary for creating a functional audio car. This means getting your motors to move. So create a program and wire up your motors to demonstrate both motors moving forward and backward and also one motor moving at a time. 



**Hint**: Take a look at [python multithreading](https://realpython.com/intro-to-python-threading/) in order to protect your program as you run methods for both motors.

To accomplish this you willl need to know how to **access and use a GPIO**

## Spectrum Analyzer (D)
If you have not used one before a Spectrum Analyzer is an instrument used to measure the magnitude of an input signal versus frequency within the full frquency range of the instrument. The primary use is to measure the power of the spectrum of known and unknown signals. For this deliverable you will use a Spectrum Analyzer (Can be found in room 1450) as you follow the instructions in this [document](./setup/spectrum_instr.md) in order to help characterize your Mic or anything else you may want to use it for. 

## Characterize Microphone(D)

For this deliverable the goal is to characterize your microphone. This means adjusting the gain(sensitivity) to your desired level. As well as testing to see what exactly your desired level is. In result you should have and LED circuit that lights up when the Microphone is picking up your sound how you want it to, as well as turning off when that sound is not in your range.


# Summary

In summary, for this week you need to:

1. **D**: Make sure all your hardware is in your kit and is in working shapes and fill out the parts checklist

2. **D**: Wiggle your DC Motors(forward, backward, and one by one).

3. **D**: Characterise your Microphone. See how sensitive it is and make sure it is characterized enough to do what you need it to with your Audio Car.

4. **D**: Practice using a spectrum analyzer, using the documents provided and provide proof in your documentation.

5. Update your User Manual and Technical Documentation with your findings.
