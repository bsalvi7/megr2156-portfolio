# A6 – Bracket Drawing Pt 1

## Objective

The objective of this project is to continue the design of the bracket made in A5. Specifically, this project aims to reference the dimensions calculated last week to make a parametric model and a detailed engineering drawing. This includes picking the dimensions that are best suited from both the stress and stiffness calculations, using the Equations tool to create a model that is defined parametrically, and using the model to create a drawing with proper dimensions and tolerances that suit the design. 

## Analyze

>Analyzing Dimension Values

I began the creation of my parametric model by first analyzing the previous dimensions I had calculated for using both stress and stiffness. By creating multi-view sketches previously, I was able to easily compare the dimensions for both calculations. For each dimension, I chose the calculation that yielded the largest value, as it would ensure that the design would not fail through either stiffness or stress. To keep track, I marked each of the values I was gonna use with a red triangle on my sketches. 

<img width="500" alt="Stress Dimensions" src="IMG_0160.jpeg" />

<img width="500" alt="Stiffness Dimensions" src="IMG_0160.jpeg" />

>Setting Up Part Creation

I then translated these values into the equation tool in Solidworks, referencing the equations I had created for each dimension in project A5. I set each of the constant values to their corresponding value in the Equation tool, and then used those variables to input the equations of each dimension, checking with my hand calculated values to ensure their accuracy. I then labeled each global variable and provided a description to make it clear what they correlated with. Features 1-5 are numbered in the order they were calculated, moving up from the cantilever beam to the hook at the top of the bracket. 

<img width="500" alt="Specs" src="1.png" />

I then went into the document properties of the part and ensured my units were set to IPS to match my previous calculations and ensure the model is accurate. Furthermore, I adjusted the decimal place that values were displayed to ensure the equations provided the result to the fourth decimal place. I also set the material to Aluminum 6061 T6, which although not utilized in this project, could prove useful later if testing is done on this model. 

<img width="500" alt="Set to IPS" src="2.png" />

<img width="500" alt="Set Material" src="3.png" />

## Decide

>Simple Features

It was now time to create the model. Features 1-3 were simple, involving sketching and dimensioning their cross-section using the parametric values I created. I then used the extrude tool to extrude them to the desired length using the parametric values. For features 1 and 2, I used the back plane of the cantilever beam to create the sketches to ensure they were aligned and defined properly without the need to create relations manually. 

<img width="500" alt="Feature 1 Sketch" src="4.png" />

<img width="500" alt="Feature 1 Extrude" src="5.png" />

<img width="500" alt="Feature 2 Sketch" src="6.png" />

<img width="500" alt="Feature 2 Extrude" src="7.png" />

<img width="500" alt="Feature 3 Sketch" src="8.png" />

<img width="500" alt="Feature 3 Extrude" src="9.png" />

>Mirrored Features

Features 4 and 5 took a few extra steps to create. I started with feature 4, creating the cross-section sketch using the back plane and extruding it to the correct length. I aligned it with the corner of feature 3 to ensure that the dimensioning was accurate with the placement of the feature. To fill in the joint between features 2 and 3, I added an extra sketch and extrude, merging the result to attach both features. 

<img width="500" alt="Feature 4 Sketch" src="10.png" />

<img width="500" alt="Feature 4 Extrude" src="11.png" />

<img width="500" alt="Joint 3-4 Sketch" src="12.png" />

<img width="500" alt="Joint 3-4 Extrude" src="13.png" />

This feature as well as feature 5 are symmetrical on both sides of the bracket. Using this relation, I was able to translate the features I created to the other side of the bracket using the mirror tool on both sketches. I drew a centerline in the middle of the bracket and used the line to mirror the sketches without the need for extra relations. Once I saved the sketch, it automatically extruded the new sketch and created a perfectly mirrored feature. 

<img width="500" alt="Feature 4 Mirror" src="14.png" />

<img width="500" alt="Joint 3-4 Mirror" src="15.png" />

I then repeated this process for feature 5, using the same method to fill the space at the joint and mirror both features. 

<img width="500" alt="Feature 5 Sketch" src="16.png" />

<img width="500" alt="Feature 5 Mirror" src="17.png" />

<img width="500" alt="Feature 5 Extrude" src="18.png" />

<img width="500" alt="Joint 4-5 Sketch" src="19.png" />

<img width="500" alt="Joint 4-5 Mirror" src="20.png" />

<img width="500" alt="Joint 4-5 Extrude" src="21.png" />

After completing feature 5, the part was complete and ready to be translated into a drawing. 

<img width="500" alt="Final Part" src="22.png" />

>Creating the Drawing

To complete the project, I created a new drawing of the part, using ANSI A Landscape as the format to best fit the model views and dimensions. I then began by laying out the front, top, right, and isometric views to set up a third angle projection drawing. For the front, top, and right views, the default 1:2 scale was about the correct size to fit the views and dimensions. I played around with the isometric view's scale, but decided that the 1:2 scale could be fit as long as it was close to the top right corner of the drawing. 

<img width="500" alt="Views" src="23.png" />

I then laid out each of the dimensions needed to define the part using the Smart Dimension tool. The front view had the most dimensions to display, so I moved each of them in a way that allowed the dimensions to not overlap or be too close to one another. The other views were less crowded, and thus were easily readable without too much movement from the standard positions of the dimensions. 

<img width="500" alt="Laying Out Dimensions" src="25.png" />

Once each of the dimensions were set on the drawing, I adjusted the decimal places on each dimensions based on their tolerance needs. For the dimensions that did not contribute to the fit of the bracket onto the rigid T-beam, I displayed up to 2 decimal places. This gives a looser tolerance of +/- .01 inches, which allows manufacturing costs to stay lower while not having huge effect on the reliability or fitment of the bracket. The safety factor applied to the calculations allows this range of error to remain acceptable. 

<img width="500" alt="Specs" src="26.png" />

The areas of contact of features 2 and 3 with the T-beam needed a much tighter tolerance in order to keep the fit with the bracket tight and not allowing excessive play or slippage. I set these to the 4th decimal place, with a set tolerance of +.0005 inches. The tolerance does not allow any value smaller than the given dimension, as a smaller value would create a press fit that would not work with a bracket system. 

<img width="500" alt="Specs" src="27.png" />

Finally, the area of contact between feature 5 and the beam could have a more lenient tolerance, as its proximity to the base of the T-beam does not affect the fitment of the bracket. I set the value to the 4th decimal place with a tolerance of -.02 inches. The positive tolerance must be zero as a longer area of contact would push the bracket away from the contact area of feature 4.

<img width="500" alt="Specs" src="28.png" />

I went into the text of the format, detailing a tolerance block as well as information about the material, manufacturing process, name and date, revision, part title, and a comment on the use of a third angle projection. 

<img width="500" alt="Specs" src="29.png" />

With this, the drawing was now compelete.

<img width="500" alt="Specs" src="30.png" />
## Communicate
>Reflections

For feature 3, I used the stiffness value to drive the value of the height of the feature in my model. This calculation used the displacement equation rearranged to solve for height h:

<img width="500" alt="Stress Dimensions" src="IMG_0162.jpeg" />

To translate this equation into CAD software, I set the constant values needed to solve the equation, including SF, F, L, E, Displacement, and b3 (a+2b of the rigid T beam). I then rewrote the equation within the Equation tool using these set variables, providing an answer that corresponded with my previous hand calculation. Although I did not make a mistake that warranted changing this or other values which connected to the equation, the importance of doing this is that the model will respond appropriately in the case of a value needing to be changed. This bypasses a complete rebuild of one or more features of the part and makes the process much more efficient. 

For feature 4's area of contact with the T-beam, I applied a tighter tolerance of +.0005 inches, while for feature 5's area of contact, I only applied a tolerance of -.02 inches. Feature 4's surface is a mating surface that ensures a proper sliding fit based on its measurement, making it critical for the fitment of the bracket onto the T-beam. This makes a tighter tolerance a more appropriate choice, as it ensures that the measurement is precise enough to create a sliding fit. On the other hand, feature 5's area of contact is not a mating surface, and only supports the bracket rather than having an effect on the bracket's fitment to the T-beam. This makes a more lenient tolerance appropriate, as it does not have any effect on the final fitment of the bracket on the T-beam while also lowering costs by not needing a highly accurate manufacturing technique. 

This assignment took me about 4 hours in total. 

CAD Parts and Drawing can be downloaded here:

<a href="A6.zip" download>
  Bracket Part and Drawing (.zip)
</a>
