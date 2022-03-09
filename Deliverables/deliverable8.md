
# Deliverable 8
In this deliverable your teams will solidify your filter design that you began the preliminary work for in Deliverable 6 and you will need to create a 2-bit ADC. This design will lay the foundation for Deliverable 9(Checkpoint 2) which is NEXT WEEK! Though there are only two things to turn in this week it is a stepping stone to what is next, look at the Minimum requirement for a 'B' on ELC and prepare for next week accordingly. 

## Helpful information on your LM339
The LM339 is open collector output.  If you haven't reviewed the LM339 data sheet or applications sheet from TI (Texas Instruments), you should (on ELC).  There are also some good links for reference on the internet to check out. However, videos and "how to" articles often leave much to the viewer/reader to consider so make sure you understand how the circuit works.  Good practice is to set up an LM339 by itself and figure out its idiosyncracies before wiring it up in your main application.
https://www.youtube.com/watch?v=b0w0q2xTzgg  
https://www.theengineeringprojects.com/2017/06/introduction-to-lm339.html



## Hardware Design for Filtering and ADC (P)

**Filter:**
Finalize and test your schematic for your filter. As a reminder, the objective of this filter is to receive sound frequencies 500Hz, 2kHZ, and 8kHz (We will test for 2kHz in this deliverable and deliverable 9) and be able to determine where that sound is so that you can move to it. Explain your filter. How does it work? How did you size component values for the desired frequency? Lastly, verify your hardware filter design; show a photo of the experimental (not simulated) Bode Plot and frequency response of the filter using the spectrum analyzer.

**Sound Steering Input:**
In order to drive to the sound, you must have a way to give direction to your PI.  The PI takes digital inputs so you will need to transform your audio filter outputs (analog) into digital which requires an analog to digital converter (ADC) of some type.  Dr Trudgen hinted that 2-bits might be sufficient.  You may use more, but over designing can make things more complicated and harder to get working. 

Your ADC will allow you to determine the strength of the sound your car is receiving and will be used to navigate to the sound source in grade checkpoint deliverable 9. Prove the schematic of your ADC works to help you differentiate the location of the sound. Explain how the ADC you made works and how it interfaces with the audio filter and with the Raspberry Pi, in an in-depth written description. 

**TURN-IN on ELC:** A document containing 1) your filter (designed for 2KHz) and ADC finalized schematic, 2) A photo of your physical hardware, 3) A written description of your filter design, including math to back up claims, 4) Photos of your physical filter response (Spectrum analyzer and Bode Plot, and 5) A written description of your ADC.  Make sure to include at least pseudo code for the PI response to the ADC input.


# Summary

In summary, for this week you need to:

1. **P:** Filter Design and Testing
2. **P:** ADC Design
3. Update your User Manual and Technical Documentation with your findings.
