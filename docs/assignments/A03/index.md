# A3: Parametric and FEA Design

## Prompt
I was given the task of designing a cantilevered bar my design class. The bar was to be designed in a CAD software of choice with a few stipulations about the design laid out as follows

- To be designed parametrically where all the values are input as equations that can changed on a whim
- Aluminum for the material
- An elastic modulus of 8.5 - 11.5 million psi that corresponds with typical values from aluminum
- An axially applied load at the unfixed end of the bar within a range of 300 lbf to 500 lbf
- A max elongation of .009 in

<img width="580" height="123" alt="image" src="https://github.com/user-attachments/assets/f892df1d-63e7-4539-8de8-50323cfbf113" />

An example diagram of the bar's setup that was given beforehand

## Hand Calculations
The first steps to take were to choose the values for the cross-section of the bar. Looking at common aluminum bar stock sizes that are readily available I decided to choose a 1/8" by 2" 6061 aluminum bar stock size. Not the smallest and something I have worked with before, it should provide plenty of area for the load ranges stated and is still fairly cheap per unit of length to acquire. Using the equations for axial elongation and axial normal stress I moved to calculating the length of my bar by hand to give the later CAD-solved numbers something to compare to.



With a length computed, it was time to move to my CAD system of choice, SOLIDWORKS, to make the bar and implement parameters for its values.
## CAD & Simulation
Like most objects the design started with making the bar itself.

<img width="842" height="739" alt="A3 base sketch" src="https://github.com/user-attachments/assets/8945bff7-79c4-404f-b183-29876ae9239a" />

Base sketch of the cross-section with width and height parameters set for their respective dimensions

<img width="1205" height="641" alt="A3 extrusion" src="https://github.com/user-attachments/assets/957343f1-d11e-48ee-90a8-b2ab75b6af35" />

Extrusion of the bar with the parameter for length later input into the dimension

<img width="1355" height="675" alt="A3 part" src="https://github.com/user-attachments/assets/310cbf5e-4992-4ced-aa27-3fb33bf377cc" />

The bar itself made of 6061 aluminum alloy in SOLIDWORKS

<img width="227" height="243" alt="A3 model tree" src="https://github.com/user-attachments/assets/044729b5-000b-4753-9595-384fecae4b8e" />

The model tree showing the material, sketches and features of the part

<img width="799" height="515" alt="A3 parameters" src="https://github.com/user-attachments/assets/676ca129-5c79-4226-9ff3-236561690c6f" />

All of the parameters stated for the part with the length variable being a rewritten elongation equation to isolate length instead. With the bar and parameters made the fixed geometry and applied force was to be added so simulations could now be run.

<img width="1255" height="628" alt="A3 fixture and load" src="https://github.com/user-attachments/assets/e09e92bb-5b19-40b7-bf9e-5830fe43fc9e" />

The fixed side and loaded side are on opposite ends of the bar

<img width="229" height="357" alt="A3 static study tree" src="https://github.com/user-attachments/assets/ead99c41-376f-4ebd-90ed-d76bbdec3a0c" />

The static study tree showing fixtures, loads, and other simulation information

<img width="1375" height="740" alt="A3 von mises" src="https://github.com/user-attachments/assets/e8c6798e-784c-4451-90a0-a049e9320785" />

First to look at with a simulation was the von Mises stress throughout the bar with a graph and maximum figure included

<img width="1352" height="720" alt="A3 displacement" src="https://github.com/user-attachments/assets/9b5028cb-56f1-4efa-881d-4aa2408bffdb" />

A displacement map showing the max elongation annotation.

With the initial study complete, the final step in CAD was to change the parameter values and go again to see how things change. Due to the nature of the elongation equation I thought that increasing the area, Modulus of Elasticity, or max elongation would increase the length and vice versa. The opposite was guessed for the force, and since I did my initial simulation a 500 lbf, the length could only go up from where it started if that was the only parameter changed.

<img width="795" height="516" alt="A3 change of height" src="https://github.com/user-attachments/assets/fba14ad6-41cb-4ef0-866c-e0efb2676d38" />

The first parameter I modified was decreasing the height which decreased the length

<img width="795" height="513" alt="A3 change of width" src="https://github.com/user-attachments/assets/383e71af-1b40-4525-a1a2-5f0804057788" />

Next I doubled the width of the bar and it also doubled the length of the bar

<img width="797" height="515" alt="A3 change of load" src="https://github.com/user-attachments/assets/aa210690-cbba-493b-83a1-a62c1cff50be" />

Last was a change in the load that saw an inversely proportional increase in length with the decrease in applied force

<img width="1252" height="796" alt="A3 von mises 2" src="https://github.com/user-attachments/assets/3e61760c-5ce1-4166-976d-629ab999d1cd" />

The von Mises map of the increase in length due to the force being lowered to 400 lbf

<img width="1204" height="791" alt="A3 displacement 2" src="https://github.com/user-attachments/assets/2cd0de56-47ec-4ee5-bd78-94ce2d9f9615" />

The displacement map of the same parameter change

## Analysis of Results

## Lessons

