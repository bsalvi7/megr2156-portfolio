# A9 – Pulleys

## Objective

The objective of this project was to design and analyze a pulley system given specifications and geometric constraints. This project required the formulation of the proper equations necessary to fully define the geometry needed for the belt, shafts, and bearings, pairing these values with an equivalent real-world part. Once the parts were determined, they were utilized to design a support for the pulley system using engineering analysis to ensure rigidity. 

## Analyze

>Given Constraints

This project provided various constraints to the design of the pulley system that I would use to calculate the undefined areas of the system. The design was a belt between two parallel pulleys that have a center distance of 4-6 inches. The pulleys have a diameter of 3 inches each, with an operating speed of 1000-2000 rpm. The belt tension under stationary conditions needed to be between 4-6 lbf, with pulleys made of aluminum, ABS, or steel and a polyurethane rubber belt. A safety factor of 3 was given. 

Before proceeding with the calculations, I decided to set the center distance to 5 inches, operating speed to 1500 rpm, and tension to 5 lbf. I also choose aluminum for the material of the pulleys. The calculations would also require a coefficient of static friction to determine the belt geometry. Using a table which provided coefficients for various polyurethane and aluminum combinations, I decided to set the coefficient of friction to 0.5 for my calculations, which sat around the middle of the range. 

<img width="500" alt="Chosen Values" src="Chosen.jpeg" />
<img width="500" alt="Friction Table" src="friction.png" />

## Decide

>Belt Design

I was now ready to determine the geometry of the belt. I began by setting my unknowns and knowns and drawing a free body diagram of the forces on the belt. Using the free body diagram, I created a statics equation and used it paired with a force-friction equation to find the two separate forces for the tight and loose end of the belt. Using these forces, I found the maximum transmitted torque and minimum cross-sectional area of the belt. I used this to determine the minimum diameter of the belt at 0.2591 inches. Using the McMaster page, I found the closest size above this minimum diameter, which was 5/16ths of an inch. I then used this value to calculate the outer circumference of the belt to fully define its geometry, finding it to be 21.39 inches. 

<img width="500" alt="Belt Calculations" src="prt1.jpeg" />

However, the McMaster page had no belts that fit both of these dimensions, meaning that I had to find a new diameter and circumference. I decided to increase the diameter to 3/8ths of an inch and recalculated the circumference, which became 21.78 inches. With this being within the range of products found in the McMaster page, I ended up picking the 3044K608 belt with a diameter of 3/8ths of an inch and a circumference of 21 inches. This slightly smaller circumference than the one calculated will allow the belt to stretch and grip firmly on the pulley surface, ensuring no slip. 

<img width="500" alt="Chosen Belt" src="belt.png" />

>Shaft Design

It was now time to design the shaft. Given a set material of AISI 1060 hardened steel, I found the yield strength to be about 82,700 psi. Similarly to the belt calculations, I set my knowns and unknowns and drew a free-body diagram, using it with a static moment equation to find the transmitted torque to equal the previously calculated value of 9.837 lbf-in. Using shear equations, I determined the symbolic representations of max and allowable shear stress, which I substituted into the minimum diameter and area equations for the shaft. Plugging in my values, I found the minimum diameter needed to be 0.154 inches. 

<img width="500" alt="Shaft Calculations" src="prt2.jpeg" />




## Communicate

