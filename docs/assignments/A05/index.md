# A5 – Bracket Design

## Prompt
The assignment for this week was to design a bracket that will slide onto a rigid support and hold a load by way of a polyester strap that distributes the load evenly across the feature it is hooked on. The focus of the assignment is to conduct dimensional analysis by use of stress and stiffness calculations and determine what material is to be used. Lastly, a second objective saw the load be applied through a linkage that attaches to where the strap would have been to a 1-inch diameter shaft, determining said dimensions through stress analysis.

**Bracket Design Stipulations**
- Make use of a Safety Factor of 4
- Applied load F in the range of 500 lbf to 800 lbf
- Choose one of three materials: 6061 T6 aluminum, ASTM A36 steel, or Ti-6Al-4V titanium
- Stiffness calculations will use a maximum deflections of .005in for each feature of a part
- Assume no failure due to direct shear stress and negligible shear deflections

**Link Design Stipulations**
- The hole that connects to the bracket must be designed as a running/sliding fit
- The hole that connects to the 1-inch diameter shaft must be designed with light assembly pressure (slight press fit)
- The connection to the 1-inch diameter shaft must be able to support the same load the bracket was designed for

Outlined from the jump were specific requirements in the design process, stated as follows:
- Each "feature" of a part will have its own free-body diagram, stress analysis, and stiffness analysis
- The reactions force from one feature of the part will act as the applied force on the next
- Model algebraic solutions and then solve numerically
- Create two separate multi-view drawings of the bracket on paper, one for each type of analysis used

## Research
I started by doing research on the mechanical properties of the materials available to choose from for the designed parts to get a grasp of how they compare. From said research, I found the following: 

<img width="513" height="120" alt="image" src="https://github.com/user-attachments/assets/ab303217-4966-4aa4-951c-4a653653e151" />

If a mechanical property is given with a range, a value near the middle is chosen for use in calculations, representing a median and likely common value found in real world use.

## Brainstorming

Having looked at the data and considering the use for the material choices above, 6061 T6 aluminum was chosen. It provides slightly better yield strength performance than ASTM A36 steel while having around a third of the weight, and in comparison to the titanium alloy option is most likely cheaper. Weight is also of importance for the object being designed will be hung and apply a load itself, something that needs to be accounted for when looking at how it supports itself and the rail it is supported by in final implementation.

<img width="3854" height="2925" alt="IMG_7894" src="https://github.com/user-attachments/assets/6dc60759-14a3-4acd-a33d-e812bb396768" />

## Calculations & Design

The flow of calculations for each feature of the object and the linkage goes as follows:
- Stress calculation including a free-body diagram of the part with two views, stating of knowns and unknowns, algebraic solution, numerical solution, conclusion of results
- Stiffness calculation with the statement of knowns and unknowns, algebraic solution, numerical solution, comparison of results between stress and stiffness, and conclusion of calculations for that feature
At the end of each feature's calculations a minimum value is stated for a critical dimension of the feature and a recommended dimension is given corresponding to easily acquirable stock sizes for the chosen material.

<img width="3965" height="2489" alt="IMG_7895" src="https://github.com/user-attachments/assets/878cde1d-8f8a-4466-8eda-ff7c6865bf04" />

<img width="4212" height="2830" alt="IMG_7896" src="https://github.com/user-attachments/assets/ebf9e66a-77a2-4db7-a147-6c6e5d841b61" />

Feature A was treated as a cantilever beam with a uniform distributed load. For a length of 1 in, a 7/8" (.875 in) diameter round bar is recommended for this feature 

<img width="3857" height="2818" alt="IMG_7897" src="https://github.com/user-attachments/assets/da93a604-d3ff-4a43-b749-cafaac275755" />

<img width="4152" height="2571" alt="IMG_7898" src="https://github.com/user-attachments/assets/bdc781d9-710a-42e2-b601-8bc29b58b346" />

Feature B was treated as an axially loaded bar in tension. With set dimensions of .875 in width and 1 in height, a thickness of 3/16" (.1875 in) is recommended for the rectangular bar.

<img width="4059" height="2299" alt="IMG_7899" src="https://github.com/user-attachments/assets/6c247010-7f36-4c68-a0a0-40dcf5a80a18" />

<img width="4122" height="2093" alt="IMG_7900" src="https://github.com/user-attachments/assets/3f2736d0-f843-44b1-8c14-91cf2491dc55" />

Feature C was treated as a simply supported beam with a concentrated load at the center. Designated as a rectangular bar with a width of 2.75 in and a length of 1 in, a thickness of 3/4" (.75 in) is recommended for the feature.

<img width="4062" height="2762" alt="IMG_7901" src="https://github.com/user-attachments/assets/24df01c1-424b-4985-aef1-1075c2686fbe" />

<img width="4126" height="2276" alt="IMG_7902" src="https://github.com/user-attachments/assets/e2713a30-1db8-4834-ba73-45fb12d61526" />

Feature D was treated as an axially loaded bar in tension like feature B. Two of the feature are required for the bracket so the total applied force of 1200 lbf was split in half for the calculations. With a set height of 1.5 in and length of 1 in, a thickness of 1/8" (.125 in) is recommended for this rectangular bar feature.

<img width="4115" height="2773" alt="IMG_7903" src="https://github.com/user-attachments/assets/35fc425e-04fb-446f-920b-0a3b734520f1" />

<img width="4231" height="2209" alt="IMG_7904" src="https://github.com/user-attachments/assets/b2893e34-97b5-451a-9a7a-abcc98a9cb39" />

Feature E was treated as a cantilever beam similar to feature A, and similar to feature D the applied force was split across two required instances of the feature in the bracket. With a set width of 1 in and a length of 1 in, a thickness of 1/2" (.500 in) is recommended for feature E.

<img width="4283" height="3621" alt="IMG_7907" src="https://github.com/user-attachments/assets/bc5cfb0b-fd63-45ec-9d8e-a86cd151f8d1" />

<img width="4283" height="2003" alt="IMG_7908" src="https://github.com/user-attachments/assets/9d7f56cc-471b-4037-9adf-8ae1579961bd" />

The hole that connects the linkage to Feature A of the bracket should be an RC2 sliding fit to allow for movement and turnability without being able to run freely, yet can handle slight changes in temperature for outdoor applications. RC2 fits typically have a +.001 in tolerance for the hole, achievable with a reaming finishing process for a Grade 7-8 standard tolerance for the 0.71-1.19 in nominal size of the hole. These selections were made from the information in Machinery's Handbook on fits and tolerances on page 650 and 651.

<img width="630" height="347" alt="image" src="https://github.com/user-attachments/assets/4202b24e-da88-4076-b2f8-487d572c32c2" />

<img width="627" height="507" alt="image" src="https://github.com/user-attachments/assets/09b02773-e866-4ccb-adb2-38b74b648be2" />

<img width="630" height="372" alt="image" src="https://github.com/user-attachments/assets/897a910e-4ec1-4752-9432-8f1b9675f301" />

The hole that connects the linkage to the 1-inch diameter shaft should be an FN1 light drive fit to fulfill the design requirement of light assembly pressure for this fit. This will in essence create a permanent fit of the linkage and 1-inch diameter shaft. This was selected with the information on page 650-652 of Machinery's Handbook, shown above and below.

<img width="625" height="592" alt="image" src="https://github.com/user-attachments/assets/9fea32b4-4b8b-484f-8945-603819904f42" />

<img width="4196" height="2216" alt="IMG_7909" src="https://github.com/user-attachments/assets/ed49f4c7-8767-41ed-86f9-60a4f0b0bbdd" />

## In Review & Lessons Learned

Looking back at this project, it was a challenge to recall the knowledge pertaining to different types of beams and beam loading scenarios. Each feature had different stipulations that required a second walkthrough of the process to ensure confidence in the following process of calculations. From the start my mind was made up to get a minimum required dimension for each feature but to recommend an actual existing stock bar size, taking knowledge from what I have heard about the design of parts used in real-world applications, what I have learned about safety factors and the over-design of parts, and when I interned at an engineering firm and saw that components are often designed or chosen with more capacity than minimally required. Following on that from engineering ethics, it just felt like the responsible thing to do to ensure safety and see the project completed fully.

The biggest lesson I learned from this project was how much time it takes to actually produce a deliverable that hits not only the requirements of the prompt but also some of my own process and deliverable additions to make the design feel more complete or language easier to understand.
