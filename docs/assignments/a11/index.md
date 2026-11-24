# A11 – Motor Selection

## Objective

The objective of this assignment is to design a motorized drive and frame for a 2 kN tensile tester. Through calculations and design work, a motor needs to be selected, confirm frame integrity, and mounting design for the motor. These design decisions will allow the smooth translation of the crosshead under a safe torque and speed for tensile tester of a high load. Pictured below are the given constraints and values for this assignment.

![Given Constraints and Values](Screenshot%202026-11-23%20205118.png)

## Analyze

>Motor Selection

For the motor selection, we used values for one half of the needed 2000 N load to find what each motor needed to provide. A 30% efficiency value was used to find a torque value that will not be overused but can still provide the needed torque to translate the crosshead vertically. With these values found, a torque of 2.695 Nm was required or 381.64 in-ozf. A RPM range of 0.197 to 9.84 was calculated to find a motor. From the McMaster website, NEMA 23 6627T923, square body motor was selected. The maximum holding torque is valued at 467.3 in-ozf and a maximum rotation speed of 300 RPM. This motor provided sufficient torque as well as RPM range for our needed values.

![Motor Calculations](IMG_3125.JPG)
![Motor Schematics](6627T923_Stepper%20MotorX.gif)
![Speed Torque Graph](6627t923-@2x_1695134526.png)


## Decide

>Bruno Salvi: Top Frame FEA

To ensure the top portion of the frame created in the previous portion of the project is able to support the loads of the motor and leadscrew, an FEA analysis was required. Taking the SolidWorks model of the top of the frame, I utilized the split line tool to allow the area where the bracket would sit to be the region where the forces were distributed. This ensured an accurate simulation by making the setup as realistic as possible.

<img width="500" alt="Sketch" src="1.png" />

<img width="500" alt="Split Line" src="2.png" />

I then applied the force of both lead screws on each region, setting each region to 1 kN. The direction was set downwards to represent the axial tension being transferred to the frame. I then applied the two separate 3.3 N*m torques in each region. Finally, I applied fixed geometry constraints to both ends of the frame to represent the top frame being mounted between both sides frame pieces. 

<img width="500" alt="Top Force" src="3.png" />

<img width="500" alt="Top Torque" src="4.png" />

<img width="500" alt="Top Fixed Geometry" src="5.png" />

I then ran the study with a coarse mesh, noting the maximum Von Mises stress, maximum displacement, and minimum factor of safety values. To ensure convergence, I ran two more iterations with increasingly finer mesh, marking the values of each. To ensure convergence, I found the percent difference of each value between iterations, ensuring that they remained within 7% for acceptable convergence. 

<img width="500" alt="Top Von Mises" src="6.png" />

<img width="500" alt="Top Displacement" src="7.png" />

<img width="500" alt="Top FOS" src="8.png" />

<img width="500" alt="Top Convergence" src="IMG_0190.jpeg" />

The maximum Von Mises stress was 8.804*10^6 N/m^2, which was far below the yield stress of the 6063-T6 aluminum the frame is made of. The displacement was under 0.01993 mm, which is acceptable given the load. Finally, the factor of safety remained well over the benchmark of 4, sitting at 24.42.

Although the design is more than strong enough to withstand the loads and torque being applied, some changes could be made to ensure consistent performance. Increasing fillet size will ensure that no stress concentrations are created in the frame. Furthermore, pocketing into the side frames can ensure that the top frame is well supported at both ends by supporting the bottom of the ends of the top frame. This will improve the performance even further. The critical location is in the middle of the beam, where it is furthest from the supports. It remains there with these changes as the load and torque remains the same. 

>Bruno Salvi: Side Frame FEA

It was now time to analyze the side frame to ensure it is strong enough. The side frame's region where loads where applied is simply at the top of the frame, meaning the split line tool is not required. Since I was only focusing on one side frame, I applied the force of one leadscrew downwards onto the top of the frame, set to 1 kN. I created an axis down the center of the side frame to reference the torque applied by the motors, setting to 3.3 N*m around the axis. Finally, I applied a fixed geometry constraint at the base of the side frame to act as the support of the ground. 

<img width="500" alt="Side Torque" src="10.png" />

<img width="500" alt="Side Fixed Geometry" src="11.png" />

I then ran the study using the same iterative method, applying a coarse mesh and noting the values. I ran the next two iterations with finer meshes and used percent difference to ensure convergence. The maximum Von Mises stress was 1.933*10^6 N/m^2 which is even lower than the top frame. The maximum displacement is 0.03271 mm, which is acceptable, and the minimum factor of safety is 111.2, which is extremely high. 

<img width="500" alt="Side Von Mises" src="12.png" />

<img width="500" alt="Side Displacement" src="13.png" />

<img width="500" alt="Side FOS" src="14.png" />

<img width="500" alt="Side Convergence" src="IMG_0191.jpeg" />

This design is very sound, but improvements could be made to it to minimize the twisting occurring. Ribbing could be incorporated into the beam to strengthen the beam against the twisting torque forces. This would be applied along the length of the beam as it is twisting laterally. The critical location would not change, as the most stress and displacement would still occur at the top of the beam where it is furthest from the fixed geometry.

Although the design is more than strong enough to withstand the loads and torque being applied, some changes could be made to ensure consistent performance. Increasing fillet size will ensure that no stress concentrations are created in the frame. Furthermore, pocketing into the side frames can ensure that the top frame is well supported at both ends by supporting the bottom of the ends of the top frame. This will improve the performance even further. Even with these changes, the critical locations will remain as the mounting point of the motor bracket where the forces are stemming from.  

CAD Parts can be downloaded here. Note that I did not include the simulation data as the file size would be too large.

<a href="Top Frame.zip" download>
  Top Frame
</a>

<a href="Side Frame.zip" download>
  Side Frame
</a>

## Communicate
