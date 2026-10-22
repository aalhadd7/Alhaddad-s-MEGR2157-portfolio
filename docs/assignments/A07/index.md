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


- **Design III – Final Modified Bracket:** [Insert CAD download link]

---

## Part 2: MEGR 2157 – Link FEA


