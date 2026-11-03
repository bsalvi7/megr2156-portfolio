# A8 – Gearbox Assembly

## Objective

The objective of this project was to design and model a two-piece gear box assembly. This included parts such as the shafts, gears, journal bearings, and housing. In the creation of the design, I analyzed and sized the input and output shafts for strength and designed journal bearings to support the shafts. To complete the assembly, I created a gearbox housing with needed clearances and fastening, using parametric CAD modeling to generate a final design. All of the steps to generate this design are documented within this page. 

## Analyze
>Given Values

This project had set values to base the calculations off of to fully define the needed specifications. This includes the gear ratio, output gear torque and speed, shaft diameters and lengths, and the exact models and details of the input and output gears. 
<img width="500" alt="Given Values" src="1.png" />

<img width="500" alt="Input Gear" src="2.png" />
<img width="500" alt="Output Gear" src="3.png" />

Assumptions are also provided that are important in the calculations. This includes assuming adequate shaft strength, ideal gear train, and negligible radial force from the gear train.

>Shaft Stress Calculations

With the given specifications, we begin by defining the specifications of the rest of the design. Using gear ratio relations, I determined the input speed and torque. With these values, it was time to confirm that the shafts are strong enough to withstand the torque and forces involved. Assuming the material of the shafts to be 1117 Carbon Steel, commonly used for shafts, I utilized stress equations to determine that the diameter of the shaft would adequately withstand the stress.  I repeated these calculations for the output shaft. For both, I determined the diameter of both shafts to be more than enough to withstand the torque and forces given a safety factor of 2. 

One thing to note is that in order to determine the bending stress of the shaft, I assumed that the shaft is supported by two journal bearings on either side. This is typical of a normal gearbox design and will continue to be utilized throughout the design. 

<img width="500" alt="Input Shaft Calculations" src="Input Shaft.jpeg" />
<img width="500" alt="Output Shaft Calculations" src="Output Shaft.jpeg" />

>Journal Bearing Calculations

Once the stress calculations were complete, I moved forward to determining the needed values of the journal bearings. Once the knowns and unknowns were listed, calculated the radial force using the previously calculated tangential force. I utilized the same journal bearing setup noted before and assumed a journal bearing length of 0.25 inches for the input and output bearings. With this setup, I calculated P and V for the input and output shaft. Using these values, I determined that Porous Bronze would be the best material to use for my journal bearings, as it meant the needed specifications while also being easy to find in many sizes and competitively cheap relative to other materials. 

<img width="500" alt="Journal Bearing Calculations" src="Journal Bearing.jpeg" />
<img width="500" alt="Materials Table" src="4.png" />

I then used Bernie's equation from the Machinery's Handbook to determine the minimum thickness needed for the input and output journal bearings. Both of these came to very small thicknesses, leaving a wide range of bronze journal bearing options available. When taking into account the length I previously specified and shaft diameters, I decided to go with 6391K111 for the input bearings and 6391K131 for the output bearings. 

<img width="500" alt="Journal Bearing Thickness Calculations" src="Journal Bearing Thickness.jpeg" />
<img width="500" alt="Input Journal Bearing" src="jb1.png" />
<img width="500" alt="Output Journal Bearing" src="jb2.png" />

>Housing Sketch

With each of the components selected, I utilized the provided dimensions to create a two piece housing design that fully encompassed the gears, bearings, and shafts. I decided to create a lip around the ends of both halves of the gearbox housing to make room for bolt holes in order to secure both halves together for efficient assembly and disassembly. 

<img width="500" alt="Gearbox Sketch" src="Gearbox Sketch.jpeg" />

## Decide

>Housing CAD Modeling

It was now time to create the gearbox assembly, beginning by bringing the gearbox housing halves in as individual models. I began by setting up my units to IPS and parametric design structure using the equations tool. These critical dimensions will be used in each of the models with the same equations tool setup.

<img width="500" alt="Units" src="6.png" />
<img width="500" alt="Equations" src="6-1.png" />

I started by modeling the front view of the top section of the housing, beginning with a rectangle. I then used the 3-point circle tool to round off the end of the housing, trimming the ends to make it one flush shape that I could then dimension. I then extruded this to the appropriate length to create the main body of the top housing.

<img width="500" alt="Rectangle" src="7.png" />
<img width="500" alt="Circle" src="7-1.png" />
<img width="500" alt="Dimensions Top Housing" src="9-1.png" />
<img width="500" alt="Extruded Top Housing" src="9-2.png" />

## Communicate

