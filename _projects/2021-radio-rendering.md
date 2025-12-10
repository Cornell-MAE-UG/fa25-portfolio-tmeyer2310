---
layout: project
title: Torque Wrench Design and Analysis
description: Engineering Materials Final Design Project
technologies: [Autodesk Fusion]
image: /assets/images/RefWrench v3.png
---

For a class, we were asked design a Torque Wrench.  

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

Nulla et magna urna. Morbi a ipsum sollicitudin, rhoncus risus volutpat, ultricies nunc. Quisque mollis finibus ante id imperdiet. Quisque vehicula elit sit amet felis facilisis fermentum.

![Dimensioned Drawing of Torque Wrench Design]({{ "/assets/images/WrenchDrawing.png" | relative_url }}){: .inline-image-r style="width: 1000px"}

Nulla et magna urna. Morbi a ipsum sollicitudin, rhoncus risus volutpat, ultricies nunc. Quisque mollis finibus ante id imperdiet. Quisque vehicula elit sit amet felis facilisis fermentum.

Aenean tincidunt aliquam arcu, in euismod dui dapibus eu. In placerat, mi et ultrices consequat, quam ligula cursus mauris, in semper neque nibh at est. Maecenas hendrerit dignissim porta. Phasellus nec fringilla dolor. Etiam efficitur nisi sit amet velit pharetra feugiat. Etiam ultrices turpis at leo semper, eleifend scelerisque neque malesuada. Aliquam molestie congue rhoncus. Donec blandit neque dolor, nec tristique mi pretium ac. Mauris tincidunt ullamcorper magna, nec pellentesque mi sagittis quis.

I was inspired by this old radio when I made this rendering:

![CAD of Torque Design]({{ "/assets/images/CADWrench.png" | relative_url }}){: .inline-image-l}

Aenean tincidunt aliquam arcu, in euismod dui dapibus eu. In placerat, mi et ultrices consequat, quam ligula cursus mauris, in semper neque nibh at est. Maecenas hendrerit dignissim porta. Phasellus nec fringilla dolor. Etiam efficitur nisi sit amet velit pharetra feugiat. Etiam ultrices turpis at leo semper, eleifend scelerisque neque malesuada. Aliquam molestie congue rhoncus. Donec blandit neque dolor, nec tristique mi pretium ac. Mauris tincidunt ullamcorper magna, nec pellentesque mi sagittis quis.

Aenean tincidunt aliquam arcu, in euismod dui dapibus eu. In placerat, mi et ultrices consequat, quam ligula cursus mauris, in semper neque nibh at est. Maecenas hendrerit dignissim porta. Phasellus nec fringilla dolor. Etiam efficitur nisi sit amet velit pharetra feugiat. Etiam ultrices turpis at leo semper, eleifend scelerisque neque malesuada. Aliquam molestie congue rhoncus. Donec blandit neque dolor, nec tristique mi pretium ac. Mauris tincidunt ullamcorper magna, nec pellentesque mi sagittis quis.
