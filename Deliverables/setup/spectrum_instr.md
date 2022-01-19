# Spectrum Analyzer Instructions

The Keysight DSOX1204G has a built-in “Frequency Response Analysis Tool”. This feature will automatically create a bode plot for your filters. 

### Hooking up: ###
Inject the signal into your circuit by connecting the “GEN OUT” BNC Jack to the input of your circuit. There are BNC cables and BNC to grabber clip adapters laying or hanging around. 
Probe the input of your circuit by connecting a 10x probe between oscilloscope channel one (yellow) and the input of your circuit. Don’t forget to ground the probe.
Probe the output of your circuit by connecting a 10x probe between oscilloscope channel two (green) and the output of your circuit.

### Prep for Analysis: ###
Press the “Analysis” button on the scope. 
Select “FRA” from the features menu by pressing the first non-descript grey rectangle button under the circular “Back” button and twisting the “Entry” knob. 
Using the other non-descript grey rectangle buttons, enter the setup menu and adjust the settings to whatever you think is appropriate.
Use the circular “Back” button to go back & hit “Run Analysis” when you feel like it. Then wait for the plot to do it’s thing.

### Unexpected Results: ###
A flat plot that starts at 0dB and rises +1 dB at ~5 Khz probably means the probes are in the wrong places. Make sure that channel one goes to the input of the circuit, and channel two goes to the output of the circuit. 
If the plot looks kinda like a janky polygraph make sure the “GEN OUT” bnc jack is connected to the input of your circuit. 


More info on [page 95](https://bkpmedia.s3.amazonaws.com/downloads/manuals/en-us/2540C_series_manual.pdf). 
