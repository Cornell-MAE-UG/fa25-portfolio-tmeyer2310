---
layout: project
title: Torque Wrench Design and Analysis
description: Engineering Materials Final Design Project
technologies: [Autodesk Fusion]
image: /assets/images/RefWrench8 v0.png
---

For a class, we were asked design a Torque Wrench. For this project, I did design requirement calculations using MATLAB, the CAD design in Fusion 360 and the FEM analysis in ANSYS Mechanical.

Requirements: 
The wrench must sustain a fully reversed torque of
  T = ±600 in-lbf for 106 cycles. 
  Design will include selecting an appropriate material and dimensions to meet or exceed the following:
    1. attain at least 1.0 mV/V output at the rated torque of 600 in-lbf
    2. safety factor of Xo = 4 for yield or brittle failure (you pick which criterion based onwhether you are using a brittle or ductile material)
    3. safety factor of XK = 2 for crack growth from an assumed crack of depth 0.04 inches (1 mm).
    4. fatigue stress safety factor of XS = 1
    5. material must be a steel, aluminum or titanium alloy.

Geometry:
L = 14;	% length from drive to where load applied (inches)  
h = 0.5;		% width   
b = 0.425;	% thickness  
c = 1.0;	% distance from center of drive to center of strain gauge  

Material Properties for AISI 4340  
E = 30.9e6;	% Young's modulus (psi)  
nu = 0.285;	% Poisson's ratio  
su = 385.e3;	% tensile strength use yield or ultimate depending on material (psi)  
KIC = 87.4e3;	% fracture toughness (psi sqrt(in))  
sfatigue = 79.e3;	% fatigue strength from Granta for 10^6 cycles  

Results (Predicted from Beam Theory Hand Calculations)
Output voltage at rated troque (600 in-lbf) = 1.0182 
Saftey Factor for Yield = 11.3628
Safety Factor for Cracking = 6.6152
Safety Factor for Fatigue = 2.3316
Deflection = 0.2866

CAD Images
![Dimensioned Drawing of Torque Wrench Design]({{ "/assets/images/RefWrench8 v0.png" | relative_url }}){: style="width:1000px;"}
Final Design Rendering

![Dimensioned Drawing of Torque Wrench Design]({{ "/assets/images/RefWrench8Drawingv0.png" | relative_url }}){:  style="width: 1000px"}
Final Design Dimensioned Drawing



![Dimensioned Drawing of Torque Wrench Design]({{ "/assets/images/TorqueWrenchV8_2.png" | relative_url }}){: style="width: 1000px"}
Fusion 360 CAD


Loading and Boundary Conditions for FEM
A force of 42.8lbf is applied in the y direction at the handle 13in from the wrench driver (in the x direction). This yields the 600 lbf-in torque. Displacement boundary conditions of 0in are set to the faces of the driver. This constrains the problem and lets us see the normal stress on the wrench in the finite element model. See image below. 
![Dimensioned Drawing of Torque Wrench Design]({{ "/assets/images/TorqueWrenchV8_Loading.png" | relative_url }}){: style="width:1000px;"}

FEM Results (ANSYS Mechanical)

![Dimensioned Drawing of Torque Wrench Design]({{ "/assets/images/TorqueWrenchV8_Strain.png" | relative_url }}){:  style="width: 1000px"}
Normal strain contours (in the strain gauge direction) from FEM
![Dimensioned Drawing of Torque Wrench Design]({{ "/assets/images/TorqueWrenchV8_PrincipleStress.png" | relative_url }}){:  style="width: 1000px"}
Contour plot of maximum principal stress from FEM


![Dimensioned Drawing of Torque Wrench Design]({{ "/assets/images/TorqueWrenchV8_StrainProbe.png" | relative_url }}){:  style="width: 1000px"}
Strain at the Strain Probe: 8.7027e-005 in/in (x-axis)

![Dimensioned Drawing of Torque Wrench Design]({{ "/assets/images/TorqueWrenchV8_Stress.png" | relative_url }}){: style="width: 1000px"}
Normal Stress: Max Normal Stress = 25455psi

![Dimensioned Drawing of Torque Wrench Design]({{ "/assets/images/TorqueWrenchV8_Displacement.png" | relative_url }}){: style="width: 1000px"}
Total Displacement: Max deflection = 0.18633

The max strain of 0.00082266in-in gives a torque sensitivity of 0.8227 mV/V.
The strain at the gauge of 8.7027e-005 gives a torque sensitivity of 0.0870 mV/V.

For the torque wrench, I would select a Bonded Resistance Strain Gauges. This strain gauge is accurate and durable and thus commonly used in torque wrenches. 


