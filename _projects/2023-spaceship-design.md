---
layout: project
title: Fluid Mechanical Dissection
description: Analysis of a Two-Stage Rocking Piston Pump
technologies: [CapCut]
image: /assets/images/IMG_5897-removebg-preview.png
---


Here is the link for the fluid mechanical disection video: 
<a href="https://drive.google.com/file/d/16spiC7umkkYN87v2Cd1uVcMVytpn6jCR/view?usp=sharin"> Here </a>

For the fluid mechanical dissection, in conjunction with my group mates, I worked on the dissasmbely of the air compressor. Specifically, I focused on the disassbly of the casing and flow frames. Together, we analyzed the fluid flow through the flow frames and discussed how the gaskets fit the sealing surfaces. I also worked on disassembling the pistons and thinking about how pressure builds up the piston chambers. In the analysis, I calcuted the Reynolds numbers at various points to see how the flow changes as the pistons compress the fluid. Finding the characteristics and the inlets and exits would allow us to better understand the flow. For the video, I recorded the voiceover and edited the final video posted (at the link above).

Below is the video script:

Script: In this video, we will be discussing the operation of the fluid mechanical components of a two-stage rocking piston pump.

Script: This machine functions as an air compressor with two rocking piston pumps in series. 

Script: The analysis in this video depends on several key assumptions. 
Assumption 1 allows us to easily characterize the pressure, density, and temperature of the ambient air. 
Assumption 2 is essential to generating time-independent analysis. 
Assumption 3 through 6 are vital to the analysis of the pistons’ compression of the air. 
Assumption 7 allows us to avoid finite element models for analysis of the cooling fan.

Script: Here we highlight the key components of the compressor, namely the cooling vent, the housing, the base, and the air intakes. 

Script: Some more key components are the cooling fan, the rotary cam, piston, and the piston cylinder

Calculations of Reynolds Number at system inlet and exit – high density at exit accounts for high reynolds number

Script: We will describe and analyze the path of the air from its ambient to compressed state. 

This shows an interior view of the top housing of the cylinder assembly. Both stages operate the same in principle, the only difference being where the air inlet and outlet connect. Air first enters in the red chamber as seen on the left and pressure is built up until the pressure force cracks the reed check valve labeled “Valve 1” with the red arrow. Air then enters the cylinder and the pressure is increased with the piston. The pressure builds in the cylinder until the pressure force is high enough to crack the reed check valve labeled “Valve 2, cylinder exit”. The air will then enter the blue chamber on the left and exit as shown either to the second stage or to the point where the pressurized air is used. 

This shows the other side of the right hand side component from the last slide (This seals the top of the cylinder). Reed check valves are simple pieces of metal that allow air to enter and exit the cylinder when a certain pressure force has been accumulated. A better side view of the valve can be seen in the schematic. 

10. We calculated the theoretical pressure increase across the pump.
We started by calculating the important volumes for the first piston. Applying the ideal gas relation assuming constant-temperature gives the pressure at the piston 1 outlet as 10.4 atm.
Next, we estimated the average velocity and Reynolds number in the tubing between the stages using the ideal gas law and conservation of mass equation. Using a moody diagram, we obtained a friction factor and calculated a pressure drop of 57 Pa across the tubing, which is negligible compared to the fluid pressure.
11. At the 2nd piston, we repeat the constant-temperature ideal gas law calculation. This results in a theoretical outlet pressure of roughly 26 bar. 
This clearly overshoots the actual measured outlet pressure of 12 bar.
Some causes for this overprediction are our assumptions of constant temperature compressions, ignoring leakage across valves and piston rings, and neglecting heat dissipation

12. Script: We will now analyze the airflow over the motor from the two airfoils on either end of the compressor.


13 Script: Here are the measurements of the cooling fan. 

14. Script: The cyan lines are streamlines representing the airflow over the motor from the spinning fans inside the housing. The fans on either end of the compressor have inverted camber. This implies that the inlet and outlet surface areas are large with low speed with high-speed flow over the motor’s smaller surface area because the streamlines over the motor are closer together. Additionally, the actuator disk model assumes that area downstream of the actuator disk is half the area of the actuator disk, implying the motor diameter is 71% of the intake diameter; thus, the motor diameter of 4.1 inches is approximately 80% of the intake and exhaust diameter of 5.1”.

Script: We care about the volumetric flow rate of air over the motor from the disks because it dictates how much heat can be dissipated. We calculate the force the disk generate using a formula developed by NASA for static thrust of a propeller in report 447. Using the definition of the pitch, P, and the pitch angle, beta, we can calculate T naught. 

Script: Here, the actuator disk model allows us to use several key assumptions, primarily that the far downstream velocity, U4, is 2 times faster than the rotor velocity, U3, and that the force is mass flow rate times U4. We can combine that with the definition of mass flow rate to compute the rotor velocity. Given the definition of volumetric flow rate, assuming standard conditions, we can compute Q to be 0.403 cubic meters per second. For a fan at 1650 RPM, this appears reasonable. 

17. The calculations shown here relate thermodynamic concepts to fluid mechanics (Calculating Re using geometry, fluid properties, and thermal parameter). The purpose of the fans is to dissipate the heat from the motor and in the cylinders during compression. To simplify calculations, we assuming the compression process is adiabatic and the only heat being dissipated is from the motor. The electrical input to the motor is 720 W and we are assuming a 80% efficient motor, where the fan is able to displace 50% of the generated heat. We solved for the heat transfer coefficient (h) to find the Reynolds number. We specifically chose the Dittus-Boelter equation because that specifies a turbulent flow through a pipe. With the Reynolds number, we calculated the diameter of the fan and obtained a value of 6.33 inches which is very close to the actual actual fan diameter of 4.8 inches. 

Script: This concludes our fluid mechanical dissection of the two-stage rocking piston pump air compressor. 
