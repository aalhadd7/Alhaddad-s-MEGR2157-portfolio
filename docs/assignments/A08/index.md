# Gearbox Design 

## Part 1: MEGR 2156 – Gearbox Design

### Introduction

For this assignment, I designed a gearbox using two spur gears, an input pinion and an output gear. The gearbox needed to be assembled and disassembled while providing enough room for the gears to rotate without contacting the housing. The given gear ratio was 24:9, with an output torque of 1.25 lb-in and an output speed of 1100 rpm. The input and output shaft diameters were 0.125 inches and 0.250 inches, respectively, with each shaft measuring 1 inch in length. I used SolidWorks to design the shafts, journal bearings, and two housing components. I also downloaded the two specified gears from McMaster-Carr and used them in my final assembly.

### Shaft Design and Calculations

I started by calculating the stresses on both shafts to determine whether their assigned diameters were sufficient. Using the gear ratio, I calculated an input speed of 2933.33 rpm and an input torque of 0.46875 lb-in. I then used the torsional shear stress equation to calculate the maximum stresses on both shafts. The input shaft had a calculated shear stress of 1222.31 psi, which was below the allowable value of 4000 psi. The output shaft had a calculated shear stress of 407.44 psi, which was below the allowable value of 8500 psi. Based on these torsional calculations, both original shaft diameters were sufficient. I also calculated the forces acting on the gears and the bearing reactions. The tangential force was 2.50 lbf, the radial force was approximately 0.91 lbf, and the resultant force was approximately 2.66 lbf. Assuming the gears were supported equally between two bearings, the radial load on each bearing was approximately 1.33 lbf.


### Journal Bearing Design and Calculations

The next step was calculating the journal bearing pressure, surface velocity, and PV values. For the input bearing, I calculated a pressure of 42.57 psi, a velocity of 95.99 ft/min, and a PV value of approximately 4086 psi-ft/min. For the output bearing, I calculated a pressure of 21.28 psi, a velocity of 71.99 ft/min, and a PV value of approximately 1532 psi-ft/min. I used these calculations as part of the bearing design process. I modeled the bearings with an inside diameter to fit the shafts and an outside diameter to fit into the housing. The input bearing was modeled with a 0.125-inch inside diameter, a 0.21875-inch outside diameter, and a length of 0.250 inches. The output bearing was modeled with a 0.250-inch inside diameter, a 0.375-inch outside diameter, and a length of 0.250 inches.

### Hand Calculations

<img width="469" height="595" alt="Screenshot 2026-10-28 at 10 36 03 PM" src="https://github.com/user-attachments/assets/aaf4e279-25e8-4458-99c5-a0dd251d7862" />


<img width="536" height="621" alt="Screenshot 2026-10-28 at 10 36 14 PM" src="https://github.com/user-attachments/assets/bec3d4b6-4eef-45e0-93bc-8e5a25709608" />


<img width="479" height="673" alt="Screenshot 2026-10-28 at 10 36 25 PM" src="https://github.com/user-attachments/assets/90a20da5-b0cd-43ac-b239-1b9fe6f8f0a4" />


<img width="533" height="662" alt="Screenshot 2026-10-28 at 10 36 38 PM" src="https://github.com/user-attachments/assets/552031f4-c412-4722-a3c4-e9bcea27c17d" />

### Input and Output Shaft Modeling

After completing the calculations, I created the two shafts in SolidWorks. I started by sketching a circle for each shaft and using the Extruded Boss/Base feature to create the required length. The input shaft had a diameter of 0.125 inches, while the output shaft had a diameter of 0.250 inches. Both were extruded to a length of 1 inch.


<img width="1086" height="534" alt="Screenshot 2026-10-28 at 10 27 53 PM" src="https://github.com/user-attachments/assets/7d178acf-7929-4622-badf-7188dc11cd00" />


<img width="1219" height="641" alt="Screenshot 2026-10-28 at 10 27 34 PM" src="https://github.com/user-attachments/assets/1e570705-abae-439c-85ed-e7746ce30153" />



### Input and Output Journal Bearing Modeling

I created the journal bearings in SolidWorks using circular sketches. I first extruded the outside diameter of each bearing, then used Extruded Cut to create the opening through the center. This allowed the shafts to fit through the bearings while maintaining the required outside dimensions.


<img width="1071" height="559" alt="Screenshot 2026-10-28 at 10 28 15 PM" src="https://github.com/user-attachments/assets/fdd7f484-daf3-4e3c-9224-899d61b01c66" />

<img width="804" height="420" alt="Screenshot 2026-10-28 at 10 28 50 PM" src="https://github.com/user-attachments/assets/3d10a74c-ff73-4e85-b37f-400ff3f57bdd" />



### Bottom Gearbox Housing

The bottom housing was the most detailed part of the design. I started by sketching a 2.50 × 2.00-inch rectangle and extruding it 0.75 inches. I then created an internal rectangular pocket using Extruded Cut, leaving material around the sides to form the housing walls. Next, I added two openings in the bottom of the housing for the input and output journal bearings. I placed the openings so the shaft centerlines were approximately 0.6875 inches apart, matching the calculated gear center distance. After creating the main housing, I added an outward extension around the upper edges to provide extra space for the mounting holes. I used Hole Wizard to create four #4 screw clearance holes, placing one near each corner of the extended area. This would allow the top and bottom housing components to be fastened together.



<img width="963" height="459" alt="Screenshot 2026-10-28 at 10 29 37 PM" src="https://github.com/user-attachments/assets/3e90dc4a-6261-4430-b88d-daa83c6f5283" />


<img width="158" height="467" alt="Screenshot 2026-10-28 at 10 29 25 PM" src="https://github.com/user-attachments/assets/210a22b4-9604-4cd2-8302-b96d47e2f5d0" />


<img width="813" height="461" alt="Screenshot 2026-10-28 at 10 29 13 PM" src="https://github.com/user-attachments/assets/ebd54b2a-7eaf-4b9f-ba0b-189798b3e4cc" />


<img width="837" height="469" alt="Screenshot 2026-10-28 at 10 28 58 PM" src="https://github.com/user-attachments/assets/e5a32ce2-b6f0-47ad-adb7-7f7973a7ea3e" />


### Top Gearbox Housing

For the top housing, I created a flat rectangular cover that would fit over the bottom housing. I used Extruded Boss/Base to create the plate and Extruded Cut to make two openings for the shafts and journal bearings. I made sure that the bearing openings matched the positions of the holes in the bottom housing. I then used Hole Wizard to create four screw clearance holes in the corners, matching the mounting holes on the bottom housing.

<img width="916" height="498" alt="Screenshot 2026-10-28 at 10 29 56 PM" src="https://github.com/user-attachments/assets/65c7b49f-a73f-4a04-b665-45d6f6a74bbc" />


<img width="953" height="590" alt="Screenshot 2026-10-28 at 10 29 48 PM" src="https://github.com/user-attachments/assets/035a16e7-af52-4be5-962c-884139ee312c" />


### Gearbox Assembly

Once the individual parts were completed, I created a new SolidWorks assembly. I inserted the top housing, bottom housing, input and output shafts, journal bearings, and the two gears downloaded from McMaster-Carr. I used concentric, coincident, and parallel mates to position the components. The shafts were aligned with their corresponding bearing openings, and the gears were positioned so their teeth would mesh together. The final assembly included both housing components, both shafts, both journal bearings, and the two spur gears. The design also included mounting holes so the housing could be secured using screws.

<img width="879" height="528" alt="Screenshot 2026-10-28 at 10 30 06 PM" src="https://github.com/user-attachments/assets/6d3ae43a-e93a-4493-8df5-cb194f85fd5e" />


### Lessons Learned

This assignment helped me better understand how individual mechanical components must fit together in an assembly. I learned how to use shaft calculations and gear dimensions to determine the placement of the parts instead of choosing their positions randomly. The most challenging part was designing the housing because I had to account for the gear spacing, bearing openings, and mounting holes. I originally started with a simple rectangular housing but later added extensions around the sides to provide enough space for the screws. I also had to make sure the openings in the top and bottom housings were aligned. Overall, this assignment improved my understanding of parametric modeling, SolidWorks assembly mates, and the importance of designing components that can be assembled and disassembled.

### SolidWorks CAD Files

The following SolidWorks part files can be downloaded:

- [Input Shaft](Input%20shaft.SLDPRT)
- [Output Shaft](output%20shaft.SLDPRT)
- [Input Journal Bearing](Input%20journal%20bearing.SLDPRT)
- [Output Journal Bearing](output%20journal%20bearing.SLDPRT)
- [Bottom Housing](bottom%20housing.SLDPRT)
- [Top Housing](top%20housing.SLDPRT)

---

## Part 2: MEGR 2157 – Engineering Drawings

### Introduction

For the MEGR 2157 portion of the assignment, I created engineering drawings of the gearbox components using SolidWorks. The drawings were made to show the dimensions and features needed to understand each part of the design. I used third-angle projection and included multiple views to show the geometry of the components. I also applied dimensioning and tolerancing conventions to the drawings.

### Shaft Drawings

I created separate engineering drawings for the input and output shafts. Each drawing shows the shaft diameter and length, along with the necessary views and dimensions. The input shaft has a diameter of 0.125 inches, while the output shaft has a diameter of 0.250 inches. Both shafts measure 1 inch in length.


### Journal Bearing Drawings

I also created engineering drawings for both journal bearings. These drawings show the inside diameter, outside diameter, and length of each bearing. These dimensions are important because the bearings must fit around the shafts and inside the gearbox housing.


### Gearbox Housing Drawings

Next, I created engineering drawings for the top and bottom housing components. The bottom housing drawing includes the overall dimensions, internal pocket, bearing openings, and mounting hole locations. The top housing drawing shows the overall dimensions, bearing openings, and four corner screw holes.

### Gearbox Assembly Drawing

Finally, I created an assembly drawing showing how the gearbox components fit together. This drawing provides an overall view of the completed design and shows the relationship between the housing, shafts, bearings, and gears.


### SolidWorks Engineering Drawing Files

The following SolidWorks drawing files can be downloaded:

- [Input Shaft Drawing](Input%20shaft.SLDDRW)
- [Output Shaft Drawing](output%20shaft.SLDDRW)
- [Input Journal Bearing Drawing](Input%20journal%20bearing.SLDDRW)
- [Output Journal Bearing Drawing](output%20journal%20bearing.SLDDRW)
- [Bottom Housing Drawing](bottom%20housing.SLDDRW)
- [Top Housing Drawing](top%20housing.SLDDRW)
- [Gearbox Assembly Drawing](Gear%20box%20assembly_Drawing.SLDDRW)
