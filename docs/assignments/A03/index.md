# Parametric Design and FEA

## 1. Parametric Design

For this project, I designed a solid circular aluminum bar under direct axial tension. I selected a load of 400 lbf, a maximum deflection of 0.009 in, a diameter of 0.50 in, and a Young's Modulus of approximately 10 × 10^6 psi.

Using the axial deformation equation, I calculated the cross-sectional area and used it to determine the required length of the bar.

My calculated values were:

- Diameter = 0.50 in
- Cross-sectional area = 0.19635 in²
- Load = 400 lbf
- Maximum deflection = 0.009 in
- Calculated length = 44.18 in
- Volume = 8.67 in³
- Weight = approximately 0.85 lb
- Normal axial stress = approximately 2.04 ksi
- Theoretical safety factor = approximately 19.6

<img width="652" height="772" alt="Screenshot 2026-09-09 at 8 26 27 PM" src="https://github.com/user-attachments/assets/42230304-959f-4d92-ae27-755f36d2e3e6" />



I then entered the design parameters as global variables in SolidWorks. The diameter, area, length, material density, and weight were linked through equations so the model could update parametrically.

<img width="884" height="482" alt="Screenshot 2026-09-09 at 7 55 09 PM" src="https://github.com/user-attachments/assets/1a45759e-71e9-416f-a9c3-72a16d224842" />


The circular sketch was created with a diameter of 0.50 in and extruded to the calculated length of 44.18 in.


<img width="852" height="439" alt="Screenshot 2026-09-09 at 7 55 32 PM" src="https://github.com/user-attachments/assets/85d85246-9d74-4689-88cf-a5bff6715d1d" />


The material selected was Aluminum 6061-T6. SolidWorks listed an elastic modulus of approximately 10.01 × 10^6 psi and a yield strength of approximately 39.89 ksi.

<img width="915" height="600" alt="Screenshot 2026-09-09 at 7 55 44 PM" src="https://github.com/user-attachments/assets/7e71a9fc-fcfe-487e-8e5f-ab35aebcaae6" />


The SolidWorks Mass Properties tool calculated a volume of 8.67 in³ and a mass of approximately 0.85 lb, which agreed closely with my calculations.

<img width="384" height="564" alt="Screenshot 2026-09-09 at 7 56 25 PM" src="https://github.com/user-attachments/assets/c5bc8e81-8305-4f81-a78c-3709c237aa90" />



## 2. Finite Element Analysis

A static FEA study was created using the same 400 lbf load used in the parametric design. One end of the bar was fixed and the 400 lbf force was applied axially to the opposite end. The material and geometry from the original design were kept the same. A mesh was generated and the study was run to determine the displacement and von Mises stress.

<img width="968" height="333" alt="Screenshot 2026-09-09 at 8 14 03 PM" src="https://github.com/user-attachments/assets/f9b17ef7-19cf-489e-8d24-7deda6dd0159" />


The displacement result was compared to the design limit of 0.009 in. The maximum von Mises stress from the FEA was approximately 2.20 ksi. You can see both the von Mises stress plot is occurring throughout the bar as well as the deflection plot:

<img width="1359" height="452" alt="Screenshot 2026-09-09 at 8 16 05 PM" src="https://github.com/user-attachments/assets/3c651d90-e535-4cbc-a35d-5ee6ff205be3" />


The aluminum yield strength was approximately 39.89 ksi, so the FEA safety factor was:

Safety Factor = 39.89 ksi / 2.20 ksi

Safety Factor ≈ 18.15

Since the maximum stress was much lower than the yield strength, the bar passed the strength requirement.


## 3. Comparison

The theoretical normal axial stress was approximately 2.04 ksi, while the FEA maximum stress was approximately 2.20 ksi. The two values were relatively close, showing that the analytical calculation and SolidWorks simulation produced similar results.

For this simple axial design, I would trust the analytical result for a quick calculation because the geometry and loading are simple. The FEA is still useful because it provides a visual representation of how stress and displacement are distributed throughout the part.

For the pin-hole portion of the assignment, the nominal stress away from the hole would be used with the appropriate stress concentration factor, Kt, to estimate the peak stress at the hole.


<img width="800" height="270" alt="Screenshot 2026-09-09 at 8 24 29 PM" src="https://github.com/user-attachments/assets/ba811aab-0a53-4ed4-9e04-8f6237ba8914" />



## 4. Lessons Learned

This project helped me better understand how load, geometry, material properties, and deflection are related. I also learned how to use global variables and equations in SolidWorks so that changing one design parameter can automatically change the dimensions of the model.

One issue I encountered was making sure the force and simulation units were entered correctly. I also had to make sure that the equations in SolidWorks matched the values from my handwritten calculations.

The total time spent completing the calculations, CAD model, simulation, and documentation was approximately 7 hours.


## 2157 Students Only – Modify Design Parameters

For the additional 2157 portion, I changed the design parameters and observed how the calculated bar length changed.

Before changing the design, my prediction was that increasing the load to 450 lbf and increasing the diameter to 0.60 in would cause the overall calculated length to increase. After changing the parameters, SolidWorks automatically updated the model through the parametric equations. This showed how changing design inputs can directly affect the final geometry without manually rebuilding the part. The material and fixture were kept the same during the modified design study.



<img width="493" height="235" alt="Screenshot 2026-09-09 at 8 30 55 PM" src="https://github.com/user-attachments/assets/5c63a6fd-0709-439e-ac36-7ae7923d9f0a" />


## CAD File

[Download the SolidWorks CAD File](./Parametric%20and%20FEA.SLDPRT)
