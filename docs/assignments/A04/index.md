# A4 – [Topic]

## Objective

The objective of this project is to create a motor mount utilizing bending equations associated with stress and displacement. Throughout the project, I got more experience navigating constraints to create a functional design and better understood how to translate a design into 3D CAD software. This project also aimed to learn how to translate dimensions into sketches that display the dimensions in a more applicable way. 

## Analyze

>Constraints and Given Values

The motor mount being designed had various constraints. The mount is designed to hold the Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox, with its dimensions being given in a drawing. 

<img width="500" alt="Motor Dimensions" src="motor.png" />

The project allowed for multiple materials to be used, including ABS, PETG, and PLA, with their properties being linked to the project page. The design contains two features, with one feature being attached to a wall and another attached to the first feature in the form of a cantilever beam, supporting the motor. Both features were to be designed with a maximum deflection of 0.3 mm at the free end with a safety factor of 3 that accounted for the holes for the screws and motor shaft. With the motor mounted, a 300N force was noted to be applied to the shaft perpendicularly. For the calculations, the weight of the motor could be ignored. Deflection of the feature attached to the wall was assumed to be zero, as well as the derivative with respect to x. 

>Design Inspriations

<img width="500" alt="Given Areas" src="Givens.jpeg" />

For design inspiration, I researched similar designs for smaller-scale electric motors. I noticed that these mounts typically had indentations which complimented the geometry of the motor it was to be used with, allowing for a more secure fit. I also noted the different mounting idea, with mounts typically using 2 or 4 screws to secure the mount. The links to these motor mounts can be found in Appendix A.

## Decide

>Defining Knowns

Before beginning calculations, I first needed to decide on my given values to set up my equations. Firstly, I needed to decide a material to use. I decided to use ABS, as not only is it very commonly used for these applications, but it is a material registered in Solidworks, allowing my material properties to be very accurate. For the ABS material, I selected a Young's Modulus of 2.5 GPa and a Yield Strength of 39 MPa to use for my calculations. I pulled these from a range of values provided in an ABS material properties table. 

<img width="500" alt="ABS Material Properties" src="0.png" />

I then needed to choose a thickness for both features. For feature 1 (cantilever) I decided on a thickness of 8mm, as it allowed for the shaft to stick out enough from the bottom of the feature while also maintaining a thickness that woudl not produce structural concerns. For feature 2 (fixed to wall) I choose a thickness of 6mm to ensure that it was thin enough to allow screws to go through the ABS material and be long enough to mount properly on the wall. 

>Solving Feature 1

<img width="500" alt="Feature 1" src="Feature1.jpeg" />
<img width="500" alt="Feature 2" src="Feature2.jpeg" />
<img width="500" alt="Given Constraints" src="Givens.jpeg" />
<img width="500" alt="Sketch" src="Sketch.jpeg" />
<img width="500" alt="Area of Bar" src="1.png" />
<img width="500" alt="Area of Bar" src="2-1.png" />
<img width="500" alt="Area of Bar" src="2-2.png" />
<img width="500" alt="Area of Bar" src="3.png" />
<img width="500" alt="Area of Bar" src="4.png" />
<img width="500" alt="Area of Bar" src="5.png" />
<img width="500" alt="Area of Bar" src="6.png" />
<img width="500" alt="Area of Bar" src="7.png" />
<img width="500" alt="Area of Bar" src="8.png" />
<img width="500" alt="Area of Bar" src="9.png" />
<img width="500" alt="Area of Bar" src="10.png" />
<img width="500" alt="Area of Bar" src="11.png" />
<img width="500" alt="Area of Bar" src="12.png" />
<img width="500" alt="Area of Bar" src="13.png" />
<img width="500" alt="Area of Bar" src="14.png" />

## Communicate

Appendix A:

https://nexusmodels.co.uk/products/j-perkins-electric-motor-mount-brush-brushless-4447205

https://bulkman3d.com/product/dc-motor-775-795-motor-mount-plate/?srsltid=AU7gw4VjQ6jf-VrZeBzc0IxJk7hn1EAzPtbX8GYxj7xmHKBHtIRepMxp
