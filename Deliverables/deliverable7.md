# Deliverable 7
In this deliverable your team will be testing out (and showing your ability) to use the microphone and ultrasonic sensor. These components will allow your team to recognize and move toward the frequencies later on. In addition, you will start your power supply design. The final design will be due as part of Deliverable 9.


## Sound Detect(P)
Have you noticed your microphone is an omnidirectional (all directions) microphone?  Clearly, it would be more desirable to have a unidirectional (one direction) microphone for this project.  Has your team thought about how to make your "omni" response more "uni" -like?  Well, if not, this is the week to do so.  Modify your setup so that the microphone is more uni-directional.  Note: As future engineers there will always be life-long learning in related fields.  

**TURN IN-On ELC**: Your team has experience using the spectrum analyzer.  Use this tool to create a video that explains: 1) how your setup became more omi-directional and 2) uses the spectrum analyzer to provide an experimental response verifying this (i.e. when you play a frequency and rotate the car it's clear that the peak magnitude strength of the response changes).  Since we will need to detect 3 frequencies, show this response for all three frequencies of interest.  (Bonus commentary: you should be thinking about how this information can help you ultimately turn left and right to move to the target.) 

## Ultrasonic Detect(P)
The microphone will help us move left and right.  Sure, it will also help us gauge distance, but we're going to use an ultrasonic sensor to further refine the distance measurement.  While future modifications will occur to your final setup, we are going to create a mini-testbed that helps us see progress. Use your wiring diagram to power the ultrasonic sensor and add code to interface it with your Raspberry Pi.  Add an LED system such that when an object is within 2 ft of the car a yellow LED turns on and when the object is within 4 inches of the car a red light turns on.  (Refer to the Project Description Document for more information).

**TURN IN-On ELC**: A short video showing that your Ultrasonic Sensor responding to objects presented to it and how close those objects are. Use LEDs to show how close the object is to the sensor.

## Power Supply(P)
Design the best power supply for your Audio Car System. Power Supply (P)
For this deliverable–and also for the next 2 deliverables– you will be working on a new power supply for your audio car. The final design will be due as part of deliverable 9. As much fun as it is to walk around your audio car with a wired power supply, it would be easier to use batteries. The power supply design that you create uses a 9V battery to power your audio car. 

**Design Specifications**:
* Power source is from a 9V battery
* Must use active components (but not special purpose IC’s) to derive the voltage(s) you need to power all components of your car.
* Filtering has been covered in this class, so a basic filter at the output will also be required to reduce noise. 
* Must have circuitry to detect Overcurrent (ie. if the battery is being shorted) and Undervoltage (ie. if the battery is running low) and warn the user. 
  * This circuitry must inform the user via LED(s). You must have 4 different states that inform the user about its diagnostic state: 


|               | Overcurrent?  | Undervoltage? |
| ------------- | ------------- | ------------- |
|       00      | No            | No            |
|       01      | Yes           | No            |
|       10      | No            | Yes           |
|       11      | Yes           | Yes           |




- Your design should optimize for size, number of components, and cost

**Long Term Submission Requirements:**
- You must submit a complete schematic and fabrication-ready board layout made with Autodesk Eagle, KiCad, Diptrace, Altium Designer, etc.
- You must also submit a MultiSim, Simulink, LTSpice, etc. simulation demonstrating the functionality, stability, and quality of your design. Your simulation should measure the output characteristics of your design with and without a load, including measurements such as voltage, current.
- In addition to your design and simulation, you'll also need to provide a Bill of Materials which should include DigiKey prices and part numbers for every electrical component.

**TURN IN-On ELC**: Submit an early design for your power supply. It can be anything from just an idea for your design, all the way up to an initial schematic or circuit diagram. Make sure you have started thinking about your power supply design. Design files can include a description (with pictures) of the design, schematics, breadboard pictures, etc.

# Summary

In summary, for this week you need to:

1. **P**: Sound Detection Demonstrated by LEDs
2. **P**: Ultrasonic Detection Demonstrated by LEDs
3. **P**: Start Power Supply Design
4. Update your User Manual and Technical Documentation with your findings.
