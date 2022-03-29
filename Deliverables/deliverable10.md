
## Inital PCB Design(P)  .
Based on your "D" checkpoint DC-DC design include and initial PCB layout.

## Initial Multifilter design (P)  .
Add 500Hz and 8KHz to your 2KHz design.  Show an initial schematic with all three frequencies handled by your hardware.  You should also show the paths to the ADC(s) for your design.  Include an initial bill of materials. for your design.  This is similar to your checkpoint 6 but with all three frequencies.  Checkpoint 11 will include bode plots of your designs.


## Finalize Power Design(D)  .

You will be required to finish Multisim/other simulation and create a Bill of Materials this week as a D design deliverable. This should allow your team to work on the PCB as part of the next checkpoint. Below is a reminder of the Design Specifications:

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




# Summary

In summary, for this week you need to:

1. **D**: Finalized Report of Power Supply Design (DC-DC) with Multisim Simulation and specific (part names, prices, vendors, values, etc), itemized Bill of Materials (BOM)
2. **P** Initial PCB design.  Eagle cad files for your DC-DC design.
3. **P**: Multifilter Design
4. Update your User Manual and Technical Documentation with your findings.
