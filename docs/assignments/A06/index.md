# Assignment 6 – Design for Strength and Stiffness II

## Bracket Parametric Design

For this assignment, I continued the bracket design from the previous strength and stiffness analysis and converted it into a parametric SolidWorks model. The final bracket dimensions were based on the dimensions selected from the previous calculations. I used A = 1.125 in, B = 0.125 in, C = 0.500 in, D = 0.125 in, and E = 0.375 in.

### Initial Bracket Geometry

I started the SolidWorks model by creating the lower portion of the bracket. I sketched the main horizontal section, the center opening, and the two stepped feet. The center opening provides the required space for the bracket to fit over the rigid T-beam. I kept the design symmetric so that changes to one side could be reflected on the other side and the geometry would remain consistent.

<img width="487" height="380" alt="Screenshot 2026-09-30 at 9 57 31 PM" src="https://github.com/user-attachments/assets/3e78c555-5100-4f9e-b2e6-04d3548a302d" />


### Main Bracket Profile

After creating the lower section, I added the upper portion of the bracket. The upper profile was created using the dimensions from my previous analysis. The outside curved portion was added to form the rounded top of the bracket.

<img width="456" height="240" alt="Screenshot 2026-09-30 at 9 58 29 PM" src="https://github.com/user-attachments/assets/7a7b2344-7e97-45ec-a550-51d4a641326f" />



The upper rounded feature was created with a radius based on Feature A. I also maintained the required wall and step dimensions around the lower portion of the bracket.

<img width="447" height="438" alt="Screenshot 2026-09-30 at 9 58 45 PM" src="https://github.com/user-attachments/assets/4b7256d7-c2a8-4f44-9caa-f5f1b0d13ebe" />


### Extruded Solid Model

Once the main profile was complete, I extruded the sketch to create the three-dimensional bracket. The extrusion created the main thickness of the part while maintaining the center opening and stepped feet.

<img width="343" height="376" alt="Screenshot 2026-09-30 at 9 59 06 PM" src="https://github.com/user-attachments/assets/abdbc394-be74-4f58-a2cf-d2f6cee27a4c" />


I then created the circular opening in the upper portion of the bracket and cut it through the entire part. This opening provides the connection point at the top of the bracket.

<img width="393" height="362" alt="Screenshot 2026-09-30 at 9 59 21 PM" src="https://github.com/user-attachments/assets/37af865a-0331-4ef8-a12d-b2c4c32862c8" />


The completed bracket contains the rounded upper connection, center opening, two support legs, and stepped feet.

<img width="398" height="395" alt="Screenshot 2026-09-30 at 9 59 34 PM" src="https://github.com/user-attachments/assets/c57cc5df-241c-4b55-a415-7bcac4bc8119" />


## Parametric Model

To make the bracket easier to modify, I created global variables in SolidWorks for the major design dimensions. The variables used were:

- A = 1.125 in
- B = 0.125 in
- C = 0.500 in
- D = 0.125 in
- E = 0.375 in

Using global variables allows the dimensions of the model to be controlled from one location instead of editing each sketch individually. This makes future changes easier and reduces the chance of inconsistent dimensions.

<img width="376" height="184" alt="Screenshot 2026-09-30 at 9 59 49 PM" src="https://github.com/user-attachments/assets/f0af1913-893a-486b-9b2b-f56e8690a398" />

The parametric setup also allows important dimensions from the previous strength and stiffness analysis to be incorporated into the CAD model. If a controlling design value changes, the corresponding parameter can be updated and the associated geometry can rebuild from that change.

## Engineering Drawing

After completing the solid model, I created a multiview engineering drawing of the bracket. The drawing includes the front view, side views, and an isometric view to clearly communicate the overall geometry of the part.

The drawing was created using third-angle projection and includes the dimensions necessary to manufacture the bracket. I also included the material as Aluminum 6061-T6 and identified the drawing as the bracket.

<img width="479" height="381" alt="Screenshot 2026-09-30 at 10 00 05 PM" src="https://github.com/user-attachments/assets/50dfae73-bdd5-4cf9-99a7-a9aee5a282c4" />


The tolerance block used on the drawing was:

- X.X ± 0.02 in
- X.XX ± 0.01 in
- X.XXX ± 0.005 in

These general tolerances provide different levels of dimensional control depending on the precision shown on the drawing. Dimensions associated with functional interfaces require greater control than dimensions that do not directly affect the fit of the bracket.

## Mistakes and Changes

One issue I encountered while creating the bracket was determining how the different dimensions from the previous strength and stiffness analysis should be represented in the SolidWorks model. I initially focused only on creating the overall shape, but the assignment required the important dimensions to also function as parameters. I corrected this by creating global variables for Features A through E.

Another challenge was creating the center opening and stepped feet while keeping the bracket symmetric. I used dimensions and sketch relations to keep the left and right sides consistent. This reduced the number of independent dimensions and made the model easier to modify.

## Lessons Learned

This assignment showed me the difference between simply creating a CAD model and creating a parametric engineering model. A normal model can have the correct dimensions, but a parametric model also preserves the relationships between the design calculations and the geometry. Using global variables makes it easier to update the design without manually changing several different sketches or features.

I also learned that tolerances should be selected based on the function of a feature. A mating or sliding surface requires more control because dimensional variation directly affects whether the components will fit together. A non-critical exterior feature can use a looser tolerance because small dimensional changes will not affect the operation of the bracket. Applying unnecessarily tight tolerances to every feature would make the part more difficult and more expensive to manufacture without improving its function.

Creating the engineering drawing also reinforced the importance of using multiple views. The front view communicates most of the bracket geometry, while the side views show the thickness and the isometric view helps communicate the overall shape of the finished part.

## Time Spent

Total time spent completing the assignment: 4 hours


## CAD Files

The completed SolidWorks files for this assignment are linked below.

[Download the SolidWorks Part](./Assignment%206_CAD.SLDPRT)

[Download the SolidWorks Drawing](./Assignment%206_drawing.SLDDRW)
