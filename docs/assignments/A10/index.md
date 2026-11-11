# A10: Lead Screw Design

## Leadscrew Diameter (Ameer Alhaddad)

For this assignment, our group was tasked with designing a tensile tester capable of applying a maximum tensile load of 2,000 N. The design uses two identical leadscrews, so I assumed the load would be distributed equally, resulting in 1,000 N per leadscrew. The required factor of safety is 4, and the crosshead must move at a speed between 1 and 50 mm/min. My assigned responsibilities were to determine the minimum leadscrew diameter, calculate the rotational speed range and maximum torque, and select a compatible leadscrew and bronze flange nut.

### 1. Determine the Minimum Leadscrew Diameter

#### Knowns, Unknowns, and Free-Body Diagram

<img width="694" height="865" alt="Unknown" src="https://github.com/user-attachments/assets/33e30fd3-bd1d-42a2-aa50-08c1acb759c2" />


#### Symbolic Solution, Numerical Solution, and Stress Verification

<img width="620" height="789" alt="Unknown-1" src="https://github.com/user-attachments/assets/5440ce9a-da7f-4990-8f2d-c289491dab3c" />


#### Explanation

I started by selecting AISI 1018 low-carbon steel for the leadscrew because it is a commonly available material for mechanical components. I researched its material properties and used a reference yield strength of 220 MPa. Using the axial stress equation and the required factor of safety of 4, I calculated a minimum leadscrew diameter of **4.81 mm**. I then checked the axial stress using a reference root diameter of 15.44 mm for a 3/4"-10 ACME leadscrew. The calculated axial stress was **5.34 MPa**, which was lower than the allowable stress of 55 MPa. This showed that the selected diameter satisfied the axial stress requirement under the assumed material properties.

### 2. Determine the Rotational Speed Range

#### Knowns, Unknowns, Free-Body Diagram, and Calculations

<img width="611" height="781" alt="Unknown-6" src="https://github.com/user-attachments/assets/af3b68e0-506f-4e30-8ebe-982e5c7f7c1c" />


#### Explanation

Next, I determined the rotational speed required to move the crosshead between 1 and 50 mm/min. I used a single-start 3/4"-10 ACME leadscrew, which has 10 threads per inch. I converted the pitch to 2.54 mm and determined that the lead was also 2.54 mm per revolution because the screw has only one thread start. Using the relationship between linear speed, rotational speed, and lead, I calculated a minimum rotational speed of **0.39 RPM** and a maximum rotational speed of **19.69 RPM**. These results established the rotational speed range needed for the leadscrews to achieve the required crosshead movement.

### 3. Determine the Maximum Leadscrew Torque

#### Knowns, Unknowns, Free-Body Diagram, and Symbolic Solution

<img width="620" height="785" alt="Unknown-2" src="https://github.com/user-attachments/assets/d44890bb-90c7-4f6b-8410-c9e26565235b" />


#### Numerical Solution

<img width="618" height="326" alt="Unknown-3" src="https://github.com/user-attachments/assets/e697588b-b89b-4a8a-a52e-6e3b0ce8af7d" />

#### Friction Coefficient Reference

<img width="764" height="434" alt="Unknown-7" src="https://github.com/user-attachments/assets/f43743b7-0c0c-4556-a738-a612b4c080d0" />

#### Explanation

After calculating the rotational speed range, I determined the torque required to rotate the leadscrews while supporting the 1,000 N axial load per screw. I used the screw torque equation from *Engineering Mechanics: Statics*, Chapter 6, Section 6/5, and calculated the mean radius, helix angle, and friction angle using the selected leadscrew dimensions. To determine the coefficient of friction, I researched the contact between steel and bronze using Roton Products' friction coefficient table. I found that lubricated steel-on-bronze contact has a coefficient of friction of **0.15**, which I used under the assumption that the leadscrew and nut would be lubricated during operation. Using the textbook equation, I calculated a torque of **1.75 N·m per leadscrew**, giving a combined torque of **3.50 N·m** for the two leadscrews. This result uses the textbook's simplified square-thread torque model, so the actual torque for the selected ACME threads may be slightly different.

### 4. Select the Leadscrew

#### Selected Component: McMaster-Carr #99030A030

<img width="2048" height="973" alt="Unknown-8" src="https://github.com/user-attachments/assets/7f1c5204-5401-4d76-896c-bbee34be4f20" />

#### Explanation

After completing the diameter, speed, and torque calculations, I selected the **1018 low-carbon steel precision ACME leadscrew, McMaster-Carr part #99030A030**. The selected leadscrew has a 3/4"-10 ACME thread, a length of 36 inches, and a single-start thread with a lead of 2.54 mm per revolution. I selected this component because its diameter exceeds the calculated minimum diameter of 4.81 mm, its length exceeds the required minimum of 18 inches, and its lead allows the crosshead to operate within the required speed range. Both leadscrews will be identical, as specified in the assignment.

---

## Select a Nut and Flange (Ameer Alhaddad)

### 1. Select and Verify the Bronze Flange Nut

#### Selected Component: McMaster-Carr #97790A140
<img width="2047" height="1000" alt="Unknown-9" src="https://github.com/user-attachments/assets/dd6e0edf-4e32-4c8c-9944-20d19951b9b7" />

#### Component Selection

I selected the **932 bearing bronze ACME flange nut, McMaster-Carr part #97790A140**, because its 3/4"-10 ACME thread matches the selected leadscrew. The nut has a length of 2.25 inches and a published dynamic thrust capacity of 2,800 lbf. After selecting the component, I performed bearing and bending stress calculations to evaluate whether its internal threads could support the applied load while meeting the required factor of safety of 4.

#### Knowns, Unknowns, and Free-Body Diagram

<img width="611" height="775" alt="Unknown-4" src="https://github.com/user-attachments/assets/d22e26a8-d6af-40b3-a052-417802a71232" />

#### Symbolic and Numerical Calculations

<img width="611" height="794" alt="Unknown-5" src="https://github.com/user-attachments/assets/1b2979b5-4533-47b5-aeae-5932e330b4ab" />

#### Material Properties and Thread Load Distribution

I started by researching the mechanical properties of 932 bearing bronze and found a reference yield strength of **14 ksi, or 96.53 MPa**, from St. Paul Foundry. I then researched how the applied load is distributed among the internal threads of a nut. According to *Shigley's Mechanical Engineering Design*, Chapter 8, Section 8-2, the engaged threads do not share the load equally, and experimental findings indicate that the first engaged thread may carry approximately 38% of the total load. Based on this reference, I used a load-distribution factor of **k = 0.38** to estimate the force acting on the most heavily loaded thread. Multiplying the 1,000 N load by 0.38 gave a first-thread load of **380 N**. This factor is a published experimental approximation rather than a measured value for our selected nut.

#### Bearing and Bending Stress Verification

Using the thread bearing and bending stress equations from *Shigley's Mechanical Engineering Design*, I calculated the stresses acting on the first engaged thread. The calculated bearing stress was **5.36 MPa**, while the bending stress was **17.31 MPa**. I then used the reference bronze yield strength of 96.53 MPa and the required factor of safety of 4 to calculate an allowable stress of **24.13 MPa**. Since the calculated bending stress was below the allowable stress, the selected nut passed the preliminary bending stress check. I also calculated an actual bending safety factor of **5.58**, which exceeded the required factor of safety of 4. These calculations use simplified thread geometry and reference material properties, so the results support the nut as a preliminary selection rather than a final manufacturer-certified verification.

---

## Sources and Part Links


### Selected Components

- [McMaster-Carr – 1018 Steel ACME Leadscrew #99030A030](https://www.mcmaster.com/99030A030)
- [McMaster-Carr – Bronze ACME Flange Nut #97790A140](https://www.mcmaster.com/97790A140)

### Material Properties

- [AISI 1018 Steel – Mechanical Properties](https://www.rootanalysis.co.uk/materials/steel/aisi-1018)
- [C93200 Bronze – Yield Strength (St. Paul Foundry)](https://www.stpaulfoundry.com/AlloySpecs/alloy_specifications_data_page.aspx?id=C93200)

### Engineering Calculations and References

- [Engineering Mechanics: Statics – Chapter 6, Section 6/5, Screws](https://studylib.net/doc/27042527/j.l.-meriam--l.g.-kraige--j.-n.-bolton---engineering-mech)
- [Roton Products – Friction Coefficients](https://www.roton.com/screw-university/screw-actions/)
- [Shigley's Mechanical Engineering Design – Chapter 8, Thread Stress and Load Distribution](https://eng.sut.ac.th/me/2014/document/MachineDesign1/document/Ch_8.pdf)
- [Rockford Ball Screw – Reference ACME Screw Dimensions](https://dpk3n3gg92jwt.cloudfront.net/domains/rockford.ballscrew/pdf/RBS_3-4_ACME_PG1.pdf)




