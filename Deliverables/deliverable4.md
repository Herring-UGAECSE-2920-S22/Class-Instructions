
# Deliverable 4
For deliverable 4, you will be programming your audio car's motors to be used at the same rate of speed using a transfer function. **Hint:** It may be a good idea to check out speed control for GPIOs. In addition you will also be illustration and describing your power diagram and GPIOS.

## Transfer Function (P)
Once you have both of your motors moving, you may have noticed that they do not move at the same rate of speed. In this deliverable you will fix this. You will need to use your optical encoders along with the to calculate a transfer function that will get both of your DC motors moving at the same RPM. You can test this by running your car in a straight line and making sure it does not veer to the left or to the right. 

**TURN IN-On ELC**: A document including the transfer function, how you got it, why it is what it is, and how you used it to make your motors run at the same speed.
 
 **TURN IN-On GitHub**: The code you used to implement your transfer function should be pushed to github and should include comments.

## GPIO Diagram and Power Diagram (P)
This deliverable will be very helpful as you progress through this project and add more parts, use more GPIOs and start to use your raspberry pi to its full potential.

-**TURN IN-On ELC**: For the **GPIO Diagram** at minimum teams must create a diagram, chart, table, or some way to indicate: GPIO names on PI, Functional name for project, default state at power up, state used for project, pull up or pull down (if any), and switch needed to set GPIO. In this document please also include an explaination of pull up and pull down resistors and how they can be used, relate to your audio car.
 
-**TURN IN-On ELC**: For the **Power Diagram** at minimum teams must create a diagram, chart, table, or some way to list each device that requires power on the design including the:

          1. Name of the Device
          2. Pins that require power(voltage requirement and current requirement)
          3. Name of source delivering the required power (voltage and current)
          
 Along with the listing is a diagram (drawing) showing each source and each load with the voltage distribution drawn. This should be included in your documentation.
 
 ## Next Design Steps
 Although this is not a deliverable this week is a great time to begin brainstorming and documenting ideas of how you all can complete the first check point refer to the [README](../README.md) and make sure you understand the checkpoint and that your team is prepared and has enough time to complete deliverable 5 aka Figure Drawing.
 
 

# Summary

In summary, for this week you need to:

1. **P:** Using the optical encoders provided, calculate and solidify a transfer function that successfully makes both of your DC motors move at the same rate of speed. You will need to complete a one page write out for the transfer functions. How did you get it, what is it, how do you use it?

2. **P:** Draw and describe your power diagram and program GPIOs

3. Update your User Manual and Technical Documentation with your findings.
