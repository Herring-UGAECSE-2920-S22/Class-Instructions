# Deliverable 9
For Deliverable 9, you will be taking on your second checkpoint. Single Sound Detect. This check point is the **Minimum Set to be considered for a “B"** remember that passing this checkpoint does not guarantee you a B but allows you to be eligible for one. In addition to that you all will complete your Power Design with Multisim/other simulation and a Bill of Materials


## Finalize Power Design(P)  The D version of this deliverable (DC-DC power design) is now moved to Checkpoint 10.  For checkpoint 9, you will have a "P" level checkpoint.  Turn this in on ELC. 
For the "P" level deliverable as part of checkpoint 9, take your starting point from checkpoint 7 and now you should have a component level schematic at a minimum.  Post this component level schematic along with an initial bill of materials to ELC.


**Design Specifications DC-DC design**:
* Let's get mobile. Power should ultimately now come from a battery as part of the DC-DC design.  Specifically, a 9V battery(ies), but generally a family of 9V batteries is acceptable (9.6V, 9.XV, i.e. it does not have to be rated explicitly at 9.0V).  
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


## Single Sound Detect(D)
Requirements for this checkpoint are quoted from the project description:

Your car can use either the 12AC/DC adapter or 9V battery(ies).  It is up to you.

>"Your car must be able to detect a single sound frequency(2kHz) and move to it without hitting the source (4 inches). A sound source will be placed 3-5 feet from the car and in any position with respect to the car (placed by grader). The car will identify and find the sound source (sound source B).  The car will drive to the sound 
source and using the usonic sensor, stop prior to hitting the source.  The front of the car must be within 
4 inches of the source before stopping."

## CATME Review(Reminder)

# Summary

In summary, for this week you need to:

1. **P**: Power Design(DC-DC) Multisim and PCB Design with itemized Bill of Materials (BOM) (Turn this in on ELC)
2. **D**: Tracking a Single Sound complete
3. **Reminder**: CATME Review 2
4. Update your User Manual and Technical Documentation with your findings.
