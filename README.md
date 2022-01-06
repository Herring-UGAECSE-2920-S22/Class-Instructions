# Class-Instructions
Instructions for each checkpoint/module in this class, as well as helpful setup/configuration instructions. Below are the design parameters for your Audio Car, as well as some rules for the class


## Project Specifications
FIRST: MAKE SURE YOU REFERENCE THE ASSESSMENT DOCUMENT ON ELC WHICH DESCRIBES THE OUTLINE OF THE COURSEWORK AND HOW YOU CAN EXPECT TO BE ASSESSED.

Your objective this semester is to design a car which can autonomously identify, track, and move to a fixed set of audio frequencies using a Raspberry Pi 4 and the necessary accompanying hardware.



As covered later, in order to accomplish this you'll be using Python to program, two DC motors for your car. In addition to that, you will be using an H-Bridge chip to drive the motors.

Our objective is to keep your cost to a minimum. However, any additional components that  your team may need that are not supplied to you is your responsibility, and if your team “cooks” a key component (see list), your team must replace the component or receive an incomplete for the course. So pay attention to the resources, best practices, and hints mentioned on this GitHub as well as in class.

There are three key objectives in this class which will be represented by deliverables throughout the semester. Each of which will be graded based on a rubric which will be provided to you. These objectives include drawing figures, detecting a single sound frequency and moving to it, and differentiating between three different frequencies and moving to each in order. Parameters for these objectives will be listed below.

You should strive to make this work as closely to a finished product as possible, meaning doing sufficient bug testing, and making the product easy to setup/use. A part of this process is making sure your code runs on startup for the Raspberry Pi. A small writeup for how to do this can be found here.

### Drawing Figures (Deliverable 5)

### Single Sound Detect (Deliverable 9)

### Differentiate Sources (Deliverable 12)


### Submitting Work

- When submitting work for this class, it will go in the deliverable assignment folder for that week. This includes any work needed for **P** and **D** deliverables, your Weekly Project Management Report, etc. Any code for your group should remain on your group GitHub repository, and you should make sure to update this with your latest work before deliverables are due.

- When submitting pictures or videos as part of your deliverable, be sure to have your subject in focus and easily seen. Make your videos short and to the point, and make sure you don't have shaky hands while you're filming.

- When submitting writing of any kind, make sure it's clear, concise, and overall decent to read. When formatting is necessary, you can assume 1.15 line spacing, and 12 pt Times New Roman or Calibri font.

## Project Rules
- Below is a set of rules to follow while working on this project in addition to any established on the syllabus. These are generally best practices for keeping your project organized and on track.

1. ### Use Clean Wiring
- Keep your wiring clean. Avoid excessively long wires which make it impossible to trace if there is a problem and are more prone to pull out. You can either purchase wires that are pre-cut to different lengths or make them yourself.

2. ### Use Color Coding
 
- Another tip is to organize your wires so that the color matches the circuit's electrical property. This will help you identify what types of wires are which when troubleshooting your breadboard circuits. The most common wire color coding is that all POWER wires should be RED, and all GROUND wires should be BLACK.

- As you get more advanced, you can have different colors representing different voltage levels and functions. For example you can add a separate color for digital signals with 5V logic, and another for 3.3V.

- For analog circuits, you may want to have a specific color for an amplifier input or output, and yet another color to identify an ADC input.

- Besides organization, this will really help you spot mis-wirings before you apply power and potentially damage your hardware. Keep a careful lookout for RED and BLACK wires connecting to the same terminal strip, as this could indicate a short.

3. ###

### Maintaining your Group Github Repository

In order to encourage you to learn the useful skill of managing and using a Git/Github repository, we ask to keep your group repository up to date, follow the [Github Flow](https://guides.github.com/introduction/flow/) and to use Git/Github features like [issues](https://guides.github.com/features/issues/) to your advantage! More information on Git/Github and how to learn it will be provided in the deliverable instructions.

### Code Style/Conventions

- Your code should follow the commonly accepted code style conventions outlined in [PEP 8](https://www.python.org/dev/peps/pep-0008/) on the official Python website. In addition to the practices outlined in PEP 8, you should follow [Object-Oriented Programming](https://en.wikipedia.org/wiki/Object-oriented_programming) principles when necessary (we'll generally let you know if something needs to be a class) and avoid creating [monolithic](https://en.wikipedia.org/wiki/Monolithic_application) software; instead opt to break your software into smaller, more manageable and maintainable pieces.

- While mildly outlined in the PEP 8 document above, we'd like to reiterate that commenting your code is crucial to both the development and grading process. A good rule of thumb to follow is that a comment should *only* be added to answer a question that the code can't. In essence, if you follow the PEP 8 naming conventions and give your variables/objects meaningful names, it won't take very long to understand most code; in some ways, the code *becomes* the documentation. However, if you use a little optimization trick here, or implement a complicated operation/algorithm there, you should add a comment explaining your implementation or methodology.

### Class Discussion

To facilitate class discussions, we will be using this repository’s **Issues** page to post comments or questions. This is a great place to ask general questions pertaining to the course and project. You are encouraged to join the discussion but just remember to abide by the “Collaboration Policy” detailed in the course syllabus. 

To post a question or comment, see the Issues link at the top of the repository or follow this [link](https://github.com/Herring-UGAECSE-2920-22/Class-Instructions/issues). The submission process is self explanatory. 
