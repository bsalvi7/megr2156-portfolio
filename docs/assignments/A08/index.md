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

It was now time to create the gearbox assembly, beginning by bringing the gearbox housing halves in as individual models. I began by setting up my units to IPS and parametric design structure using the equations tool. These critical dimensions will be used in each of the models with the same equations tool setup. I also set the material to 6061-T6 aluminum to keep the design lightweight. 

<img width="500" alt="Units" src="6.png" />
<img width="500" alt="Equations" src="6-1.png" />

I started by modeling the front view of the top section of the housing, beginning with a rectangle. I then used the 3-point circle tool to round off the end of the housing, trimming the ends to make it one flush shape that I could then dimension. I then extruded this to the appropriate length to create the main body of the top housing.

<img width="500" alt="Rectangle" src="7.png" />
<img width="500" alt="Circle" src="7-1.png" />
<img width="500" alt="Dimensions Top Housing" src="9-1.png" />
<img width="500" alt="Extruded Top Housing" src="9-2.png" />

I then created the extrusion where the journal bearing will be seated, mirroring it across utilizing a plane at the midpoint of the main extrusion done previously. 

<img width="500" alt="Bearing Sketch" src="10-1.png" />
<img width="500" alt="Bearing Extrusion" src="10-2.png" />
<img width="500" alt="Mirror Plane" src="11.png" />
<img width="500" alt="Mirrored Bearing" src="11-1.png" />

With the main shape made, it was important to ensure the inner dimensions remained intact while also hollowing out the housing to make room for the gearbox components. To do this, I used the shell tool with the outside shell box checked to hollow out the model with a specified thickness of 0.05 inches. 

<img width="500" alt="Shell" src="13.png" />

I then made extrusion cuts for the shaft hole and hole at the bottom that will be needed to connect the input and output gears together. 

<img width="500" alt="Shaft Sketch" src="12.png" />
<img width="500" alt="Shaft Cut" src="12-1.png" />
<img width="500" alt="Bottom Sketch" src="14.png" />
<img width="500" alt="Bottom Cut" src="14-1.png" />

Now, I created the lip to connect both halves of the gearbox housing, extruding the lip and cutting four holes in either corner for bolts to be run through. I created one hole in one corner, and then used the mirror tool in combination with a referenced centerline to efficiently make the other three holes. 

<img width="500" alt="Lip Sketch" src="15.png" />
<img width="500" alt="Lip Extrude" src="15-1.png" />
<img width="500" alt="Hole Sketch" src="16.png" />
<img width="500" alt="Hole Mirror" src="16-1.png" />
<img width="500" alt="Hole Cut" src="16-2.png" />

This completed the design of the top housing. I used the exact same process to then create the bottom housing using the dimensions I noted within my sketch. 

<img width="500" alt="Top Housing Iso View" src="17.png" />
<img width="500" alt="Bottom Housing Iso View" src="19.png" />

> Shaft Models

With the housing complete, I now created the simple models of both shafts. I used the same model setup with the change of material to Plain Carbon Steel which shared similar properties to the Carbon Steel I used in my calculations. I then created the sketches and extrusions of each shaft in separate models.

<img width="500" alt="Plain Carbon Steel" src="20.png" />
<img width="500" alt="Input Shaft Sketch" src="21-1.png" />
<img width="500" alt="Output Shaft Extrude" src="21-2.png" />
<img width="500" alt="Output Shaft" src="22.png" />

> Assembly

With the housing and shaft modeled, I then downloaded each of the gear and journal bearing part models from the McMaster website. I then created an assembly file to fit each of the components together. I began with the top housing, mating each of the input journal bearings on either side of the housing. I then mated the input shaft and gear together, locking them together to accurately represent the press fit. I then aligned the shaft with the journal bearings. To define the location of the gear, I used the distance mate against the back side of the housing to make sure it is not contacting anything other than the shaft while also making its location easily repeatable for the other gear. 

<img width="500" alt="Bearing Mates" src="23.png" />
<img width="500" alt="Shaft-Gear" src="24.png" />
<img width="500" alt="Shaft-Bearing" src="25.png" />
<img width="500" alt="Lock Shaft to Gear" src="26.png" />
<img width="500" alt="Set Gear Distance" src="27.png" />

I then setup the bottom half of the gearbox in the exact same manner. To connect both halves, I mated each of the bolt holes together to perfectly align both halves together. To complete the assembly, I then setup a gear mechanical mate with the specified tooth counts to ensure the gears behave as they should when in contact with one another. 

<img width="500" alt="Bottom Half" src="28.png" />
<img width="500" alt="Aligning Halves" src="29.png" />
<img width="500" alt="Complete Assembly" src="33.png" />

## Communicate

>Lessons Learned

Throughout this project, I learned how important it is to verify the functionality of something before modeling it. One mistake that I made when creating the model was beginning the model prior to creating the sketch for the housing. This made my model go through a lot of trial and error, which led to this process of my project taking much longer than I expected. If I instead ensured my sketch was fully correct before making the model, this process of creating the model of the housing would have been far easier. Another lesson that I learned was how useful setting preliminary values can be. Much of this assignments calculations required me to assume properties or dimensions to get values, and I found that setting this value to be something realistic makes it much easier to create a design that is functional from the beginning and is only in need of optimization. In the future, I will use this to create designs that do not have the issue of not working, but instead of performance, which is much easier to refine. 

In total, this assignment took me 5 hours to complete. 

CAD Assembly can be downloaded here:

<a href="A8 Gearbox Assembly.SLDASM" download>
  Gearbox Assembly
</a>


