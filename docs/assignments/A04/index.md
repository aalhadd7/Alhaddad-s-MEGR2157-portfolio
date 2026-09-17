# Motor Mount Design

The goal of this assignment was to design a motor mount for a 24 V brushed DC gear motor while considering both bending stress and deflection. The mount was designed using PLA with a safety factor of 3 and a maximum allowable deflection of 0.30 mm. I first completed the beam calculations for the motor attachment feature and wall attachment feature, then used those results to create the final SolidWorks model. The final design was also used to create the required multiview engineering drawing for MEGR 2157.

## Question 1 - Feature 1: Motor Attachment

Feature 1 is the horizontal portion of the motor mount that supports the motor. I modeled this feature as a cantilever beam with an applied load of 300 N. My initial design used a 50 mm beam length and a 45 mm width. PLA was selected as the material with an elastic modulus of 3500 N/mm² and a yield strength of 50 N/mm². A safety factor of 3 was used, and the maximum allowable deflection was limited to 0.30 mm.

For the stress analysis, I used the rectangular beam bending equations and solved symbolically for the required thickness. The stress calculation resulted in a minimum required thickness of approximately 10.95 mm, which was rounded to 11 mm. I then completed the deflection analysis using the cantilever beam deflection equation. The deflection requirement resulted in a thickness of approximately 14.7 mm, which was rounded to 15 mm. Since the deflection requirement produced the larger thickness, deflection controlled the design of Feature 1.

### Hand Calculations - Question 1

<img width="663" height="856" alt="Screenshot 2026-09-16 at 10 30 28 PM" src="https://github.com/user-attachments/assets/58054c28-e81c-4a7a-8d6e-8f552f05367a" />

<img width="588" height="762" alt="Screenshot 2026-09-16 at 10 31 18 PM" src="https://github.com/user-attachments/assets/f7d3e74f-b4a8-4f9d-9fd3-b70dfbe664e9" />



## Question 2 - Feature 2: Wall Attachment

Feature 2 is the vertical portion of the motor mount that attaches to rigid wall A. For this feature, I used a 50 mm length and a 45 mm width. The 300 N load from Feature 1 creates a transferred bending moment of 15,000 N·mm at Feature 2. The same PLA material properties, safety factor of 3, and maximum deflection of 0.30 mm were used.

The bending stress analysis resulted in a minimum required thickness of approximately 10.95 mm. The deflection analysis for the wall feature resulted in a required thickness of approximately 16.82 mm. I rounded this value to 17 mm. Since deflection again controlled the design, Feature 2 required a 17 mm thickness. Because Feature 2 required the larger thickness, I used 17 mm as the common thickness for the final CAD model to keep the bracket consistent and conservative.

### Hand Calculations - Question 2

<img width="663" height="859" alt="Screenshot 2026-09-16 at 10 32 57 PM" src="https://github.com/user-attachments/assets/7c95e27e-6212-41cb-9f55-43b1b4dbf648" />


<img width="666" height="364" alt="Screenshot 2026-09-16 at 10 32 15 PM" src="https://github.com/user-attachments/assets/80122b00-cf1a-46e6-b0a6-0574ea25dee4" />



## Initial Motor Mount Design

After completing the calculations, I created an L-shaped motor mount using the calculated dimensions. The basic design consists of a horizontal motor mounting plate and a vertical wall mounting plate. The main bracket width was set to 45 mm, while the horizontal and vertical design lengths were based around 50 mm. A 17 mm thickness was used throughout the main bracket based on the controlling result from Feature 2.


<img width="560" height="379" alt="Screenshot 2026-09-16 at 10 41 00 PM" src="https://github.com/user-attachments/assets/c68722ff-1b1e-4819-bbf8-f0d76e1d37e5" />


## CAD Model

I created the final motor mount in SolidWorks using fully defined sketches and dimensional constraints. The main L-shaped profile was modeled first and extruded to a width of 45 mm. The 17 mm thickness used in the CAD model was selected from the calculated requirement of Feature 2. I then did an extrude boss through the Mid-Plane to get my 45 mm depth.

<img width="542" height="413" alt="Screenshot 2026-09-16 at 10 22 04 PM" src="https://github.com/user-attachments/assets/c4320a3b-3e45-4f13-914a-52c0c105c704" />

<img width="539" height="300" alt="Screenshot 2026-09-16 at 10 22 16 PM" src="https://github.com/user-attachments/assets/2938d18a-8eaf-4438-b19d-99ef025764cc" />


The motor mounting pattern was created on Feature 1. The center opening was modeled as Ø18.5 mm, and four Ø3.4 mm clearance holes were added around the center for the M3 motor mounting bolts. The four smaller holes were created using a circular sketch pattern so that the mounting pattern remained symmetric. The centers of the motor mounting holes were positioned 14 mm from the center of the main opening in my final CAD model.

<img width="544" height="464" alt="Screenshot 2026-09-16 at 10 22 26 PM" src="https://github.com/user-attachments/assets/0e8e1bf1-5f89-4da6-bab9-982a29c776a8" />


Feature 2 contains four Ø3.4 mm clearance holes for attaching the bracket to the rigid wall. The holes were positioned symmetrically so the wall attachment would distribute the load across the vertical plate.

<img width="678" height="458" alt="Screenshot 2026-09-16 at 10 48 21 PM" src="https://github.com/user-attachments/assets/9b1e5010-9de3-4a90-b418-2c3b14136b2a" />


To increase the stiffness of the motor mount and reduce deflection, I added two triangular gussets between Feature 1 and Feature 2. Each gusset was designed approximately 25 mm high by 25 mm long and was extruded 5 mm thick. These gussets reinforce the 90-degree connection between the horizontal and vertical portions of the bracket and help resist bending.


<img width="538" height="429" alt="Screenshot 2026-09-16 at 10 47 58 PM" src="https://github.com/user-attachments/assets/8eb47223-d044-436f-9a2d-bc8f8fa06bec" />


The final material was set as PLA in SolidWorks. I created a custom PLA material using an elastic modulus of 3500 N/mm² and a yield strength of 50 N/mm² so that the CAD material properties remained consistent with the values used in my handwritten calculations.

<img width="752" height="548" alt="Screenshot 2026-09-16 at 10 42 51 PM" src="https://github.com/user-attachments/assets/41718cef-ec99-4a66-9f14-84c853c91978" />


### CAD File Download

The completed SolidWorks part file can be downloaded below.

[Download the SolidWorks CAD File](Assignment%204%20CAD.SLDPRT)


## MEGR 2157 - Engineering Drawing

For the MEGR 2157 portion of the assignment, I created a multiview engineering drawing from the finished CAD model. The drawing includes the required front, top, right-side, and isometric views. Center marks were added to the circular features, and hole callouts were used for the Ø3.4 mm mounting holes. Important dimensions such as the 17 mm thickness, 45 mm width, 50 mm dimensions, and Ø18.5 mm center opening were included so the part can be understood and manufactured from the drawing.

The title block identifies the part as the Motor Mount, lists PLA as the material, and includes my name, date, scale, and drawing number. The finished drawing was exported as a PDF for submission.


<img width="756" height="583" alt="Screenshot 2026-09-16 at 10 23 27 PM" src="https://github.com/user-attachments/assets/0f202568-a46a-42c8-b59d-3c5913a3cb76" />


### SolidWorks Drawing File

[Download the SolidWorks Drawing File](Assignment%204%20Drawing.SLDDRW)


## Problems and Changes During the Design

One issue I encountered was determining the correct placement of the reinforcement gussets. My first gusset sketches were placed on the outside of the bracket, which caused the extrusion to either extend outside the part or become hidden inside existing material. I corrected this by moving the gussets into the open inside corner between Feature 1 and Feature 2. This created visible triangular reinforcements connecting the horizontal and vertical plates.

I also had to carefully separate the dimensions that came from the beam calculations from the dimensions required to fit the actual motor. The beam calculations determined the required plate thickness, while the motor dimensions controlled the center opening and bolt-hole geometry. This helped me understand that structural sizing and component-fit dimensions serve different purposes in the same design.

## Lessons Learned

This assignment helped me understand how stress and deflection calculations directly influence a CAD design. Although the stress calculations produced acceptable dimensions, deflection controlled both Feature 1 and Feature 2 and therefore determined the final thickness of the bracket. I also learned how gussets can significantly improve the stiffness of a bracket without simply increasing the thickness of the entire design. On the SolidWorks side, I gained more experience using fully defined sketches, circular sketch patterns, cut extrudes, boss extrudes, custom materials, and engineering drawings.

## Time to Complete

The total time required to complete the calculations, CAD model, revisions, and engineering drawing was approximately 9 hours.

## Appendix - Motor Mount Research

Before completing the design, I reviewed examples of motor mounting brackets to better understand common mounting arrangements and methods used to reinforce L-shaped brackets.

(https://www.omc-stepperonline.com/brushed-24v-dc-gear-motor-3-6kg-cm-46rpm-w-99-5-1-planetary-gearbox-pa28-28245800-g100)
