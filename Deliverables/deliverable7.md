# Deliverable 7
In this deliverable you will be testing out and showing your ability to use the Microphone as well as the Ultrasonic sensor. These components will allow you to recognize and move toward the frequencies at the end of this project. In addition you will start your power supply–and also for the next 2 deliverables– you will be working on a new power supply for your audio car. The final design will be due as part of deliverable 9. As much fun as it is to walk around your audio car with a wired power supply, it would be easier to use batteries. The power supply design that you create uses a 9V battery to power your audio car. 


## Sound Detect(P)
For this part of the deliverable your task is to detect specific frequencies using your microphone. One easy way to show that your microphone is detecting sound is to use LEDs in combination with your GPIOs on your raspberry pi. See how sensitive you microphone is, how loud of a speaker you may need to use (Phone/Laptop/Speaker/etc.), and whether your microphone responds to all 3 sounds required for the final check point(refer to README). This sound detection will be very important as you get ready for your next big checkpoint after spring break: Single Sound Detect.

Your microphone is an omnidirectional (all directions) microphone.  It would be more desirable to have a unidirectional (one direction) microphone for this project.  Has your team thought about how to make your "omni" more "uni" -like?

**TURN IN-On ELC**: A short video showing that your microphone responds to all 3 frequencies and the strength of the sound as the sound moves around the "front" of the microphone.  This is forcing you to think about sound and direction. Use LEDs to show how the sound level changes as it passes the microphone.(**HINT:** Louder sound more LEDs lit).

## Ultrasonic Detect(P)
This part will be similar to the one before, your task is to test your ultrasonic sensor and be able to detect when an object is within 4 inches of your car, you will need this capability for the final checkpoint.(Refer to the Project Description Document for more information).

**TURN IN-On ELC**: A short video showing that your Ultrasonic Sensor responds  to objects presented to it and how close those objects are. Use LEDs to show how close the object is to the sensor(**HINT:** Closer the object more LEDs lit).

## Power Supply(P)
Design the best power supply for your Audio Car System. Power Supply (P)
For this deliverable–and also for the next 2 deliverables– you will be working on a new power supply for your audio car. The final design will be due as part of deliverable 9. As much fun as it is to walk around your audio car with a wired power supply, it would be easier to use batteries. The power supply design that you create uses a 9V battery to power your audio car. 

**Design Specifications**:
* Power source is from a 9V battery
* Must use active components (but not special purpose IC’s) to derive the voltage(s) you need to power all components of your car.
* Filtering has also been covered in this class, so a basic filter will also be required. 
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
