# Assignment 7 – Finite Element Analysis (FEA)

## Part 1: MEGR 2156 – Bracket FEA

### Introduction

For this assignment, I used Finite Element Analysis (FEA) in SolidWorks to test and improve the bracket I created in Assignment 6. The goal was to make the bracket stronger and stiffer while keeping it as lightweight as possible. I started with my original design, ran simulations to see how it performed, and then made modifications based on the results. I tested three different designs and compared their maximum stress, deflection, mass, safety factor, and number of mesh elements.

Throughout the process, I kept the same 6061-T6 aluminum material and used a 1 N force applied to the curved upper surface of the bracket. I also used fixed geometry at the mounting surfaces to keep the simulation conditions consistent.

### Design I – Original Bracket

I started by opening my original bracket in SolidWorks and creating a static stress study. I applied the force to the curved upper section and fixed the mounting surfaces at the bottom of the bracket. After setting up the simulation, I created the first mesh and ran the analysis to examine the stress, strain, displacement, and safety factor.

<img width="1019" height="579" alt="Unknown-1" src="https://github.com/user-attachments/assets/3c4ef881-b682-46fb-a425-ca23ae3f27b1" />


<img width="2048" height="1112" alt="Unknown-3" src="https://github.com/user-attachments/assets/884c28e1-9e3f-4ace-9cd7-4b86c4698b89" />


After completing the first simulation, I refined the mesh to see how the results changed as the number of elements increased. My first run contained 8,925 elements, followed by 25,489 elements for the second run and 69,732 elements for the third run. I compared the results between runs to check whether they were within the required 7% difference.

<img width="2048" height="946" alt="Unknown-4" src="https://github.com/user-attachments/assets/97a362ce-f532-4220-9dff-6346678c9597" />

<img width="1017" height="454" alt="Unknown-2" src="https://github.com/user-attachments/assets/ce62d19f-759a-4bb9-b2ba-2bc36b0143b1" />

<img width="2048" height="986" alt="Unknown-5" src="https://github.com/user-attachments/assets/98685bdc-8f60-4650-89aa-f754b1c67d33" />

<img width="668" height="694" alt="Screenshot 2026-10-21 at 11 06 22 PM" src="https://github.com/user-attachments/assets/8e2d9d34-7e4a-490c-ab8d-cd8b7f02b4dd" />



The final mesh produced a maximum von Mises stress of 29,530 N/m², a maximum deflection of 8.02 × 10⁻⁷ mm, and a minimum safety factor of 9,314. The mass of the bracket was approximately 0.01 lb. Although the deflection results were consistent between the finer meshes, the stress and safety factor did not converge within 7%. Following the assignment instructions, I used the finest mesh after the third run.

<img width="2048" height="966" alt="Unknown-6" src="https://github.com/user-attachments/assets/ea7628fb-858e-4012-b8c2-fc34fa327604" />


After reviewing the results, I decided to modify the sharp corners near the supporting legs to see whether adding fillets would improve the bracket's performance.

### Design II – Adding Fillets

For my second design, I kept the original bracket geometry but added 0.06-inch radius fillets near the legs and mounting transitions. I made this change to reduce the sharp corners and see whether the stress would distribute more evenly throughout the bracket.

<img width="1014" height="522" alt="Unknown-8" src="https://github.com/user-attachments/assets/d86471d3-c294-45b1-947f-cc8f68778d23" />




I then created another static simulation using the same material, applied force, and fixed geometry. Just like the first design, I began with a coarse mesh and gradually increased the number of elements. The first run contained 2,428 elements, the second contained 8,893 elements, and the third contained 70,110 elements.

<img width="919" height="487" alt="Unknown-13" src="https://github.com/user-attachments/assets/29b8b2bf-1b85-4e42-aafc-540f7a871c1a" />


<img width="1022" height="411" alt="Unknown-9" src="https://github.com/user-attachments/assets/6803fff5-0db0-4f3c-bac9-ffee9adfe32e" />

<img width="1005" height="439" alt="Unknown-10" src="https://github.com/user-attachments/assets/673df7ce-88a5-46fc-9175-20ee5b88af87" />


<img width="1024" height="411" alt="Unknown-11" src="https://github.com/user-attachments/assets/0fe44b05-e2c5-4b69-80dc-ef107b9eb636" />


<img width="868" height="830" alt="Screenshot 2026-10-21 at 11 06 52 PM" src="https://github.com/user-attachments/assets/b2405c1c-7cc2-4c81-97ae-390e4b773483" />



After the third run, the maximum stress was 29,610 N/m², the maximum deflection was 8.02 × 10⁻⁷ mm, and the minimum safety factor was 9,287. The mass remained approximately 0.01 lb. The stress and safety factor still did not converge within 7%, so I used the finest mesh results as instructed.

<img width="945" height="496" alt="Unknown-14" src="https://github.com/user-attachments/assets/30556c33-c599-4610-91cd-89b556ea548b" />


<img width="996" height="444" alt="Unknown-12" src="https://github.com/user-attachments/assets/c6f0fb45-fb47-4e16-8197-b34b3ced12cb" />


Comparing Design II with the original bracket, I found that the fillets did not produce a noticeable improvement in the final results. The maximum stress increased slightly, while the deflection remained almost the same. This showed me that adding fillets does not automatically improve a design, especially when the modifications are made in areas that may not be experiencing the highest stress.

### Design III – Increasing Thickness and Adding Additional Fillets

For my third design, I decided to make a larger change to the bracket. I initially increased the extrusion thickness to 0.50 inches using the Mid Plane option in SolidWorks. However, after checking the mass, I noticed that it increased significantly compared with the previous designs. Since one of the goals of the assignment was to keep the component lightweight, I reduced the extrusion thickness to 0.35 inches.

I also added 0.06-inch radius fillets along the bottom interior edges and supporting areas of the bracket. I wanted to test whether increasing the thickness and smoothing the inside corners would improve its strength and stiffness.

<img width="979" height="551" alt="Unknown-15" src="https://github.com/user-attachments/assets/fabea9d6-76d0-4849-802f-ec8e771e8f2f" />

After making these changes, I created another static simulation with the same material and loading conditions. I started with a coarse mesh containing 5,151 elements and then refined it to 9,754 elements for the second run.

<img width="971" height="451" alt="Unknown-16" src="https://github.com/user-attachments/assets/2b6380a6-039a-42c3-8f93-9d526cc3481c" />

<img width="1006" height="399" alt="Unknown-17" src="https://github.com/user-attachments/assets/8d2a1b1b-906e-448e-939f-49af70b6c37a" />


<img width="2048" height="944" alt="Unknown-18" src="https://github.com/user-attachments/assets/42b0ee10-c905-47dc-a9ed-115d73dcccde" />


<img width="937" height="485" alt="Unknown-19" src="https://github.com/user-attachments/assets/8cfe13e9-b877-4471-981d-836ff0759281" />




The second run produced a maximum von Mises stress of 41,430 N/m², a maximum deflection of 5.177 × 10⁻⁶ mm, and a minimum safety factor of 6,638. The bracket's mass increased to approximately 0.02 lb.

Unlike the previous two designs, Design III met the 7% convergence requirement after the second run. The maximum stress changed by approximately 4.86%, the deflection changed by 0.46%, and the safety factor changed by 4.63%. Because all three values were within 7%, I did not need to perform a third mesh run.

Although Design III achieved mesh convergence, its overall performance was not necessarily better than the previous designs. The bracket had more mass, and the recorded maximum stress and displacement were higher. This helped me understand that increasing the thickness of a component does not always result in a better design, especially when weight is also an important consideration.

<img width="616" height="637" alt="Screenshot 2026-10-21 at 11 07 12 PM" src="https://github.com/user-attachments/assets/070f47d3-f93a-4004-93c9-c7489a64be8c" />


### Final Design Comparison

After completing the simulations, I compared the final results from each of the three designs. For Designs I and II, I used the finest mesh results after three runs. For Design III, I used the second run because the results had already converged within 7%.

| Measurement | Design I | Design II | Design III |
|---|---|---|---|
| Maximum Stress (N/m²) | 29,530 | 29,610 | 41,430 |
| Maximum Deflection (mm) | 8.02 × 10⁻⁷ | 8.02 × 10⁻⁷ | 5.177 × 10⁻⁶ |
| Mass (lb) | 0.01 | 0.01 | 0.02 |
| Minimum Safety Factor | 9,314 | 9,287 | 6,638 |
| Number of Elements | 69,732 | 70,110 | 9,754 |


Based on the final recorded results, Design I performed slightly better than Design II in terms of maximum stress and safety factor, although their results were very close. Design III was heavier and experienced higher stress and displacement. However, the first two designs did not fully converge, so their differences should be interpreted carefully.

### Mistakes and Challenges

One of the main challenges I encountered was achieving mesh convergence. For the first two designs, I continued making the mesh finer, but the maximum stress and safety factor continued changing by more than the required 7%. This meant I had to use the finest mesh after the third run instead of stopping because the results had converged.

Another challenge was finding a balance between strength and weight. When I initially increased the thickness of Design III to 0.50 inches, the mass increased significantly. I realized that adding too much material went against the lightweight requirement, so I reduced the thickness to 0.35 inches before continuing with the simulations.

### Lessons Learned

This assignment helped me understand how Finite Element Analysis can be used to evaluate a design before making physical changes to it. I learned that the number of mesh elements can affect the stress and safety factor results, which is why refining the mesh and checking convergence are important parts of the process. I also learned that a finer mesh generally requires more computational effort.

Another lesson was that a design that looks stronger is not necessarily more efficient. Adding fillets to my second design did not significantly improve the results, and increasing the thickness for my third design increased the weight without producing the improvement I expected. Comparing all three designs helped me understand why engineers need to consider stress, deflection, safety factor, and mass together rather than focusing on only one measurement.

### Time Spent

On this Lab I spent approximately 5 hours. With majority of the work begin already completed in the previous lab. Once I got comfortable working the mesh system on solid works the work flow became much faster for me.   

### CAD File

The SolidWorks CAD files for the final bracket design is available below.

- [Download Bracket CAD File](Assignment%206_CAD_3.SLDPRT)

---

# Part 2: MEGR 2157 – Link FEA

### Introduction

For the second part of this assignment, I created a link component in SolidWorks and performed Finite Element Analysis (FEA) to evaluate its strength and stiffness. The goal was to understand how the link responds to an applied force and how changing the mesh size affects the simulation results. Similar to the bracket portion, I analyzed the maximum stress, strain, deflection, and safety factor while checking for the required 7% mesh convergence.

### Link Design and Simulation Setup

I started by creating a simple connecting link with two circular holes, one at each end. I used 6061-T6 aluminum, the same material from the bracket portion of the assignment. After finishing the model, I created a static stress study in SolidWorks Simulation.

For the simulation, I applied fixed geometry to the inside surface of the smaller hole and a 1 N force to the inside surface of the larger hole. This allowed me to examine how the link behaves when one end is supported and the other experiences a load.



### First Simulation – Coarse Mesh

I began by generating a coarse mesh and running the first simulation. The mesh contained 1,402 elements, and I recorded the maximum von Mises stress, strain, deflection, and minimum safety factor.

The first run produced a maximum stress of 8.639 × 10³ N/m², a maximum strain of 9.705 × 10⁻⁸, and a maximum deflection of 7.150 × 10⁻⁷ mm. The minimum safety factor was 3.183 × 10⁴, and the mass of the link was 47.71 g.

<img width="998" height="468" alt="Unknown-20" src="https://github.com/user-attachments/assets/d0f8ec23-7cb4-4e12-a50c-6aad9878ec75" />


<img width="2048" height="739" alt="Unknown-21" src="https://github.com/user-attachments/assets/1513a4f4-4436-49cc-9346-c854557f1fc8" />


<img width="2048" height="769" alt="Unknown-22" src="https://github.com/user-attachments/assets/dffeef1c-d436-454d-ac3c-2f4454cd0a01" />


<img width="2048" height="844" alt="Unknown-23" src="https://github.com/user-attachments/assets/4681eb0b-41c5-4117-ba82-6c3ea62c98eb" />


Looking at the stress plot, I noticed that the highest stress occurred around the larger hole where the force was applied. Most of the middle section experienced relatively low stress. The displacement plot also showed greater movement near the loaded end, while the fixed end remained restrained.

### Second Simulation – Finer Mesh

After recording the first results, I refined the mesh to determine whether the calculated values would change significantly. The second mesh contained 13,256 elements, giving the simulation more elements to represent the geometry of the link.

<img width="2048" height="861" alt="Unknown-24" src="https://github.com/user-attachments/assets/9217c12b-65de-4004-a44d-3ff54c98dbd3" />


The second simulation produced a maximum von Mises stress of 8.623 × 10³ N/m², a maximum strain of 9.944 × 10⁻⁸, and a maximum deflection of 6.781 × 10⁻⁷ mm. The minimum safety factor was 3.189 × 10⁴, while the mass remained 47.71 g.

<img width="670" height="422" alt="Screenshot 2026-10-21 at 11 07 21 PM" src="https://github.com/user-attachments/assets/8f34041e-5896-4536-a2c9-e989ac75f92d" />


### Mesh Convergence Results

After completing the second simulation, I compared the results with the first run to determine whether they were within the required 7% difference.

| Measurement | Run 1 – Coarse | Run 2 – Finer | % Change |
|---|---|---|---|
| Maximum Stress (N/m²) | 8.639 × 10³ | 8.623 × 10³ | 0.19% |
| Maximum Strain | 9.705 × 10⁻⁸ | 9.944 × 10⁻⁸ | 2.46% |
| Maximum Deflection (mm) | 7.150 × 10⁻⁷ | 6.781 × 10⁻⁷ | 5.16% |
| Mass (g) | 47.71 | 47.71 | 0% |
| Minimum Safety Factor | 3.183 × 10⁴ | 3.189 × 10⁴ | 0.19% |
| Number of Elements | 1,402 | 13,256 |

To calculate the percentage change, I used the difference between the new and previous results, divided by the previous result, and multiplied by 100.

All the results were within the required 7% difference. The stress changed by only 0.19%, the deflection changed by 5.16%, and the safety factor changed by 0.19%. Since the results met the convergence requirement, I used the second run as my final mesh for the original link.

### Results and Observations

After comparing both simulations, I noticed that increasing the number of mesh elements did not significantly change the overall results. The stress remained concentrated around the larger hole where the load was applied, and the smaller hole stayed restrained by the fixed geometry.

The minimum safety factor was approximately 31,890, indicating that the link was well below the material's yielding limit under the applied 1 N load. The deflection was also extremely small. These results showed that the original link was relatively stiff and had a large margin against yielding under the simulated conditions.

### Mistakes and Challenges

One challenge I encountered was determining where to apply the fixture and force. Since the link has two holes, I needed to decide how to represent its support and loading conditions. I fixed one hole and applied the load to the other before running the simulation.

Another challenge was understanding the effect of mesh refinement. I initially started with a coarse mesh, but I needed another simulation to check whether the results were accurate enough to use. After increasing the number of elements, I compared the values and found that the results were within the required 7% difference.

### Lessons Learned

This part of the assignment helped me understand how FEA can be applied to a connecting link. I learned that the location of the applied load and the fixed geometry influences how stress and displacement are distributed throughout a component.

I also learned that using more mesh elements does not always result in a major change in the calculated values. My second simulation had significantly more elements than the first, but the maximum stress and safety factor changed by less than 1%. This showed me why checking convergence is important instead of assuming that the finest possible mesh is always necessary.

Overall, analyzing the link helped me better understand how SolidWorks Simulation can be used to evaluate a component's mechanical performance before manufacturing it.

### Time Spent

**[Insert actual time spent modeling the link, running the simulations, and documenting the results]**

### CAD File

The SolidWorks CAD file for the link is available below.

[Download Link CAD File](link_1.SLDPRT)


