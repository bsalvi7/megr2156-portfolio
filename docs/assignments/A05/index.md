# A5 – Bracket Design

## Objective
This project tasked me to create a bracket to hold a symmetrically applied horizontal force via a strap. This bracket must have its dimensions designed with different fit classes in mind. 

The objective of this project is primarily to add stiffness analysis as a tool to be used to create engineering designs. Throughout this project, I will continue to follow the familiar strategy of creating free body diagrams of each element, identifying knowns and unknowns, stating assumptions, and performing stress analysis. However, I will now also complete this process using stiffness analysis as well, given deflection constraints. I can then compare the two results and reflect on how their results compare. 

## Analyze

>Specifications

The design of the bracket revolved around the specifications of the rigid body that it would attach to. The rigid body had specific dimensions given with tolerances, which I determined would lead me with a choice on how to approach the clearance fits of each feature of the bracket. Beyond these dimensions, the force range that the strap would apply was also given, ranging from 500 lbF to 800 lbF. Furthermore, a safety factor of 4 was given to be applied to all calculations for each feature's dimensions. I was also given a choice between three materials, including aluminum 6061 T6, Steel (ASTM A36), or Titanium (Ti-6A1-V4). When calculating the dimensions based on stiffness, a deflection of 0.005 inches waws given to be used for each feature. 

<img width="500" alt="Specs" src="Analyze.png" />

The appendix of the document I was provided also gave a tip on how to approach the design of the bracket, splitting it into 5 features that needed to be designed:
- Cantilever beam supporting the strap
- Connecting rod to bracket body
- Base of bracket
- Sides of bracket
- Hooks of bracket

By keeping the design symmetrical, it allows the sides and hooks of the bracket to fall under one set of calculations. 

## Decide

>Finalizing Specifications

My first decision was to choose the specifications I was given a choice on. Firstly, I decided to use a force of 600 lbF to create a design that would sit in the middle ground of the force range. However, I went a bit lighter in order to have a slimmer and more compact design after calculations, as a smaller load would not demand features that were very bulky in size. Secondly, I decided to use 6061 T6 aluminum to incorporate a compact design with a light material. The material properties of this aluminum were easily locatable online. 

<img width="500" alt="Aluminum Properties" src="Al Props.png" />

>Solving the Stress-Oriented Design

With these decisions made, it was now time to begin calculations with stress in mind. Taking the maximum yield strength from the property table and the other given and decided specifications, I started with the cantilever beam holding the strap and planned to work my way up the design. Firstly, I picked the length of the beam to be 2 inches as a starting point for the rest of the design, giving more than enough space for a strap to be fully supported by the beam. I began by writing the knowns, unknowns, and assumptions made for the calculation. Then, I drew a free body diagram which showcased the load (blue) and subsequent reaction forces (red). In this particular feature, it is possible to show the load of the strap as a distributed load due to its characteristics. Using stress relations, I calculated the minimum diameter needed to fall under the stress limit given the safety factor. 

<img width="500" alt="Feature 1 Stress" src="Stress 1.jpeg" />

The reaction forces of the bar then were translated into the second feature; the connecting rod. For the rest of the features, I continued to right knowns, unknowns, and assumptions while also creating a free body diagram with loads determined by the previous features reactions and the reactions of the current feature .I decided to give its width the same dimension as the diameter of the bar in order for them to connect to each other smoothly when assembled. I then utilized tensile stress equations to determine the minimum area, connecting that with the width to determine the base dimension. 

<img width="500" alt="Feature 2 Stress" src="Stress 2.jpeg" />

For the next three features, I used bending beam equations, choosing a base or width based on the dimensions of the rigid body to fully define the feature for calculations. For each of these chosen dimensions, I decided to add .0005 inches to the dimensions of the rigid body in order to create a clearance fit. The clearance fit allows the bracket to fit smoothly onto the rigid body, ensuring that the bracket is not to tight to where it cannot slide freely on the rigid body. I also picked a length of 2 inches for each of these features to align them with the length of the bar supporting the strap. This allows the design to remain balanced in its weight by centering its weight, allowing the bracket to slide more easily and be more stable. With this completed, I utilized the bending stress equations to find the final needed dimension for each feature, completing the design of the stress-oriented bracket. 

<img width="500" alt="Feature 3 Stress" src="Stress 3.jpeg" />
<img width="500" alt="Feature 4 Stress" src="Stress 4.jpeg" />
<img width="500" alt="Feature 5 Stress" src="Stress 5.jpeg" />

>Solving the Stiffness-Oriented Design

The stiffness design carried over many of the same values and mechanics of the stress design. For each feature, I was able to carry over the specifications, chosen dimensions, assumptions, and free body diagrams, making this step a much faster process. This time, I instead used the aluminum's Young's Modulus value over the yield strength to solve the equations. For each of these calculations I used relations with the given deflection and moment of inertia to solve for the needed dimensions. In this step, bending did not require extra calculations for moment, which also sped up the process of solving for the dimensions. 

<img width="500" alt="Feature 1 Stiffness" src="Stiff 1.jpeg" />
<img width="500" alt="Feature 2 Stiffness" src="Stiff 2.jpeg" />
<img width="500" alt="Feature 3 Stiffness" src="Stiff 3.jpeg" />
<img width="500" alt="Feature 4 Stiffness" src="Stiff 4.jpeg" />
<img width="500" alt="Feature 5 Stiffness" src="Stiff 5.jpeg" />

>Creating Multiview Sketches

With both the stress and stiffness designs fully defined, I could now create Multiview sketches of each to lay the dimensions and design out in a more digestible fashion. For both sketches, I created a front, right, and top view, with an isometric sketch to make the design easier to understand. For the moment, I left it dimensionless and created two copies in order to serve as a baseline for both sketches. I then laid out each of the dimensions on the view that they fit the best in, ensuring that what they were referring to was visible in the view they were populated in. With the dimensions set for each, I then referenced the dimensions to scale the design in a way that was more true to the given dimensions, allowing the difference between both designs to be more easily noticeable. 

<img width="500" alt="Stress Sketch" src="Stress Sketch.jpeg" />
<img width="500" alt="Stiffness Sketch" src="Stiff Sketch.jpeg" />

Laying both sketches side by side make it much more simple to compare how the designs differ. The most noticeable difference is in the final feature, where the height of the hooks are noticeably larger, possibly meaning that the stiffness required there is much higher relative to the stress it is undergoing, making it thicker in the stiffness design to account for that. 

## Communicate

