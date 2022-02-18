# Deliverable 7
In this deliverable your team will be testing out (and showing your ability) to use the microphone and ultrasonic sensor. These components will allow your team to recognize and move toward the frequencies later on. In addition, you will start your power supply design. The final design will be due as part of Deliverable 9.


## Sound Detect(P)
Have you noticed your microphone is an omnidirectional (all directions) microphone?  Clearly, it would be more desirable to have a unidirectional (one direction) microphone for this project.  Has your team thought about how to make your "omni" response more "uni" -like?  Well, if not, this is the week to do so.  Modify your setup so that the microphone is more uni-directional.  Note: As future engineers there will always be life-long learning in related fields.  

**TURN IN-On ELC**: Your team has experience using the spectrum analyzer.  Use this tool to create a video that explains: 1) how your setup became more omni-directional and 2) uses the spectrum analyzer to provide an experimental response verifying this (i.e. when you play a frequency and rotate the car it's clear that the peak magnitude strength of the response changes).  Since we will need to detect 3 frequencies, show this response for all three frequencies of interest.  (Bonus commentary: you should be thinking about how this information can help you in code ultimately turn left and right to move to the target.) 

## Ultrasonic Detect(P)
The microphone will help us move left and right.  Sure, it will also help us gauge distance, but we're going to use an ultrasonic sensor to further refine the distance measurement.  While future modifications will occur to your final setup, we are going to create a mini-testbed that helps us see progress. Use your wiring diagram to power the ultrasonic sensor and add code to interface it with your Raspberry Pi.  Add an LED system such that when an object is within 2 ft of the car a yellow LED turns on and when the object is within 4 inches of the car a red light turns on.  (Refer to the Project Description Document for more information).  

**TURN IN-On ELC**: Create a short video showing that your Ultrasonic Sensor responds to objects presented to it.  Use the practice LEDs to show distance.  

## Power Supply(P)
One of Dr. Trudgen's favorite words is **iteration:** a procedure in which repetition of a sequence of operations yields results successively closer to a desired result.  Often in electronic projects the first iteration uses benchtop power supplies.  For our project, essentially this was the 12V 5A power supply brick that was supplied with the project.  It is now time to iterate and design a power supply that matches the desired mobility of the car.  This design will start here and finish in Deliverable 9.  

**Design Specifications**:
* Let's get mobile.  Power should ultimately now come from a battery.  Specifically, a 9V battery(ies), but generally a family of 9V batteries is acceptable (9.6V, 9.XV, i.e. it does not have to be rated explicitly at 9.0V).  
* Your team will need to choose an acceptable battery.  Let's think about what an acceptable battery is:  1) this is not a mechanical engineering design class, but we've all had physics.  Your chosen battery still needs to be able to be physically mounted to the car chassis.  So weight and size are definitely considerations.  2) We are going with the 'RC car model'.  Did you ever (or maybe still do) play with an electric RC car?  You get about 15mins out of them when ran hard.  So, your team will need to think about current draw to size the battery such that the audio car can operate for 15 mins.  Also, since engineering is not about feelings, but calculations, make sure to include all relevant calculations and technical assumptions.  3)  In the spirit of the thrifty-ness of the audio car, cost minimization is a consideration to include.  
* Your design must use active components (but not special purpose IC’s) to derive the voltage(s) you need to power *all components of your car.
* Filtering has been covered in this class, so a basic filter at the output will also be required to reduce noise. What filter should be used?  Well, first you'll need to consider the impedance of your battery.  
* Your design must have circuitry to detect overcurrent (ie. if the battery is being shorted) and undervoltage (ie. if the battery is running low) and warn the user. Here overcurrent is defined as any value greater or equal to 1A, and undervoltage is any battery potential less than or equal to 7V.  
  * To alert the user of either of these states, build and LED system with the following diagonstic logic:  


|               | Overcurrent?  | Undervoltage? |
| ------------- | ------------- | ------------- |
|       00      | No            | No            |
|       01      | Yes           | No            |
|       10      | No            | Yes           |
|       11      | Yes           | Yes           |


* The best designs will minimize: cost, size, components and maximize: performance, length of operation, and ease of manufacturing.  

**Long Term Submission Requirements:**
- You must submit a complete schematic and fabrication-ready board layout made with Autodesk Eagle, KiCad, Diptrace, Altium Designer, etc.
- You must also submit a MultiSim, Simulink, LTSpice, etc. simulation demonstrating the functionality, stability, and quality of your design. Your simulation should measure the output characteristics of your design with and without a load, including measurements such as voltage, current.
- In addition to your design and simulation, you'll also need to provide a Bill of Materials which should include DigiKey prices and part numbers for every electrical component.
- Finally, you should evaluate the efficiency of your power supply solution.  Make sure you understand what that means and how to evaluate.

**TURN IN-On ELC**: For Deliverable 7, use the lecture on functional decomposition.  Your team needs to provide a nearly completed level 0 and level 1 design for the power supply.  You are not selecting the components yet, that would be level 2.  

# Summary

In summary, for this week you need to complete:

1. **P**: Microphone tests to make the behavior more uni-directional.  
2. **P**: Get the ultrasonic sensor working and demonstrate its functionality with LEDs.  
3. **P**: Start Power Supply Design by submitting nearly completed Level 0 and 1 functional decomposition.  
4. Update your User Manual and Technical Documentation with your findings.
