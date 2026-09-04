# A2 – Truss Stress Analysis

## Objective

The objective of this assignment was to design and analyze a lightweight planar truss capable of safely supporting the required loads. I completed the design by selecting a truss geometry, creating free body diagrams, calculating the internal member forces, determining the required sizes of the truss members and connecting pins, and creating the final design in SolidWorks. This process connected the hand calculations to a physical CAD model while considering structural safety, weight, and the required factors of safety.

For my design, I selected the following parameters:

- Applied load: **P = 20 kN**
- Horizontal dimension: **a = 0.4 m**
- Vertical dimension: **b = 0.3 m**
- Truss material: **A500 structural steel**
- Truss member factor of safety: **3.5**
- Pin material: **Hardened tool steel**
- Pin shear yield strength: **170 ksi**
- Pin factor of safety: **4**
- Pin connection: **Single shear**

---

## Analyze

### Question 2 – Truss Design and Analysis

For my truss design, I used five joints labeled **A, B, C, D, and E** and seven members connecting the joints. I analyzed the structure by drawing the overall free body diagram and individual joint free body diagrams, then using static equilibrium and the method of joints to determine the internal forces. This analysis allowed me to determine which members were in tension or compression and identify the member carrying the largest internal force.

After finding the internal forces, I used the largest force along with the material yield strength and required factor of safety of **3.5** to determine the minimum cross-sectional area of the members. I then selected a **15 mm × 15 mm square cross section** for all members, giving an actual area of **225 mm²**. Using the same cross section for every member satisfies the assignment requirement for identical member cross-sectional geometry and provides an area greater than the calculated minimum.

The final part of Question 2 was estimating the weight of the truss. I determined the lengths of the individual members and used the total material volume and steel density to estimate the weight. This hand-calculated value was later compared with the SolidWorks Mass Properties result.

#### Question 2 – Complete Hand Calculations

The following handwritten work contains my truss geometry, overall free body diagram, individual joint free body diagrams, symbolic solutions, numerical internal-force calculations, cross-sectional area calculation, and approximate truss weight.

<img width="680" height="844" alt="Screenshot 2026-09-03 at 7 54 46 PM" src="https://github.com/user-attachments/assets/5500e2c8-1610-403e-9a7b-78d20531323e" />

<img width="672" height="775" alt="Screenshot 2026-09-03 at 7 55 18 PM" src="https://github.com/user-attachments/assets/23f15832-24a9-4758-8247-3c0957d1fdf9" />

<img width="571" height="845" alt="Screenshot 2026-09-03 at 7 55 39 PM" src="https://github.com/user-attachments/assets/d991ccec-ca29-4ab6-b867-cee7343b6479" />

<img width="589" height="827" alt="Screenshot 2026-09-03 at 7 55 57 PM" src="https://github.com/user-attachments/assets/50499f07-514c-401b-8a79-b27b175deb0d" />

---

### Question 3 – Pin Design and Analysis

I designed the connecting pins to safely withstand the forces transferred through the truss joints. The pins were analyzed as **single-shear connections** using the specified hardened tool steel shear yield strength of **170 ksi** and the required factor of safety of **4**. I first identified the pin with the largest expected load and used that load to determine the minimum required cross-sectional area.

The calculated minimum pin area was approximately **68.25 mm²**, corresponding to a minimum cylindrical pin diameter of approximately **9.32 mm**. I selected a **10 mm diameter pin**, which provides a cross-sectional area of approximately **78.54 mm²**. The 10 mm diameter was selected because it is larger than the calculated minimum and provides a practical whole-millimeter dimension for the SolidWorks model.

I also estimated the combined weight of the pins using their dimensions and the specified material density. The same selected pin dimensions were then carried into the CAD portion of the assignment. This kept the physical CAD design consistent with the dimensions established through the hand calculations.

#### Question 3 – Complete Hand Calculations

The following handwritten work contains my known and unknown quantities, free body diagram of the critical pin, symbolic solution, numerical cross-sectional area calculation, selected pin diameter, and approximate combined weight of the pins.

<img width="578" height="868" alt="Screenshot 2026-09-03 at 7 56 46 PM" src="https://github.com/user-attachments/assets/0ce574fd-f2f3-49f1-94dc-072eccab3b79" />

<img width="677" height="632" alt="Screenshot 2026-09-03 at 7 57 10 PM" src="https://github.com/user-attachments/assets/97bbfc7a-08f1-4eb0-b2e3-1a5d7fc254ec" />


---

### Question 4 – SolidWorks CAD Model

I created the final 3D truss model in SolidWorks using the geometry and dimensions established through my calculations. The truss, excluding the pins, was modeled as one part, and each structural member was created using the same **15 mm × 15 mm cross section**. Creating the CAD model allowed me to convert the analytical design into a complete three-dimensional representation and verify that the selected dimensions could be incorporated into the final geometry.

The pin holes were created at each connection point, and the pins were modeled as cylindrical components using the selected **10 mm diameter**. The same pin size was used at each joint to maintain consistency throughout the design. Material was maintained around the pin locations so that the required member cross section was not reduced at the connections.

#### SolidWorks Truss Model

<img width="716" height="374" alt="Screenshot 2026-09-03 at 8 04 19 PM" src="https://github.com/user-attachments/assets/e808938a-b82a-441c-a911-ed3d5e1af4cd" />


### Mass Properties

After completing the truss geometry, I assigned the selected steel material and used the SolidWorks **Mass Properties** tool to determine the predicted mass and volume. After the pin holes were cut from the model, SolidWorks calculated a truss mass of **3,843 g (3.843 kg)** and a volume of **488,377 mm³**. I used these results to evaluate the final CAD design and compare it with the approximate weight determined from my hand calculations.

The CAD model accounts for the exact geometry of the truss, including the intersections between members and the material removed for the pin holes. Because the hand calculation uses simplified member geometry, some difference between the hand-calculated and SolidWorks values is expected. This comparison provided a way to check the analytical estimate against the final three-dimensional model.


<img width="312" height="473" alt="Screenshot 2026-09-03 at 8 03 36 PM" src="https://github.com/user-attachments/assets/851c9bf7-bae5-46fe-b90c-12f2cb2f5f9f" />


---

## Decide

### Truss Geometry Selection

I selected a truss geometry consisting of five joints and seven members, with diagonal members forming triangular sections between the upper and lower joints. I chose this configuration because the diagonal members provide paths for transferring the applied loads at the lower joints toward the supports while maintaining a stable structure. I also kept the geometry relatively simple to limit unnecessary members and reduce the amount of material used in the final design.

<img width="514" height="328" alt="Screenshot 2026-09-03 at 8 05 49 PM" src="https://github.com/user-attachments/assets/8ec2702e-581d-45e2-9a69-3dbdc36b0447" />


### Member Size Selection

I selected a **15 mm × 15 mm square cross section** for all of the truss members based on the minimum area determined in Question 2. The selected cross-sectional area of **225 mm²** is greater than the calculated minimum required area and satisfies the required factor of safety. I also selected a square cross section because it provides consistent geometry for every member and was straightforward to reproduce in SolidWorks.

### Pin Size Selection

I selected a **10 mm diameter** for all connecting pins after calculating a minimum required diameter of approximately **9.32 mm**. The selected diameter provides more cross-sectional area than the calculated minimum while remaining close to the minimum size needed for the design. Using the same 10 mm pin at every joint also satisfies the requirement that the connecting pins be identical.

---

## Communicate

### Engineering Lessons Learned

This assignment helped me understand how the geometry of a truss affects the internal forces carried by its individual members. By creating free body diagrams and applying static equilibrium, I was able to determine which members were in tension or compression and identify the critical member. This showed me why the internal forces must be determined before selecting the dimensions of structural members.

I also learned how factors of safety affect engineering design decisions. Instead of sizing the truss members and pins directly at their theoretical failure limits, I used the required factors of safety to establish minimum dimensions and then selected practical dimensions above those minimum values. This resulted in the selection of **15 mm × 15 mm members** and **10 mm diameter pins**.

Creating the design in SolidWorks also showed me how analytical calculations connect to an actual CAD model. The dimensions determined from the calculations were used to create the final geometry, while the Mass Properties tool provided the predicted mass and volume of the completed truss. Comparing the CAD results with the hand calculations helped demonstrate how a simplified analytical model relates to the exact geometry of a three-dimensional design.

### Final Design

The final design combines the truss analysis, member sizing, pin analysis, and CAD modeling into one complete engineering design. The dimensions of the members and pins were selected based on the calculated loading and required factors of safety rather than appearance alone. The completed SolidWorks model represents the final result of the design decisions and calculations performed throughout the assignment.

<img width="806" height="326" alt="Screenshot 2026-09-03 at 8 07 13 PM" src="https://github.com/user-attachments/assets/a25c0721-6480-4202-822b-2b44034eaa52" />


### CAD Files


---

## Failure Mode Analysis

### Part 1 – Truss Members

The truss members can experience different failure modes depending on whether they are subjected to tension or compression. The structural steel used for the truss is treated as a **ductile material**, so tension members would be expected to experience yielding before fracture as the axial stress increases. The largest calculated member stress was approximately **71.2 MPa** based on the selected **225 mm²** member cross section.

For members subjected to compression, **buckling** is an important potential failure mode because a slender member can become unstable before the material reaches its compressive yield strength. The likelihood of buckling depends on factors such as the member length, cross-sectional geometry, stiffness, and end conditions. Increasing the moment of inertia of a compression member or reducing its unsupported length would increase its resistance to buckling.

For members subjected to tension, the likelihood of yielding could be reduced by increasing the cross-sectional area. A larger area would reduce the normal stress produced by the same axial force. This would allow the member to withstand a larger applied load before reaching the material yield strength.

### Part 2 – Pin Connections

The expected failure mode of the connecting pins is **shear yielding** because the pins were designed as single-shear connections. The specified hardened tool steel has a shear yield strength of **170 ksi**, and the required factor of safety for the pin design is **4**. My calculations resulted in a minimum pin diameter of approximately **9.32 mm**, so I selected a **10 mm diameter pin** for the final design.

The selected 10 mm pin has a cross-sectional area of approximately **78.54 mm²**, which is greater than the calculated minimum area of approximately **68.25 mm²**. This provides sufficient shear area for the design loading based on the specified material strength and factor of safety. The complete calculations and comparison are shown in my handwritten Question 3 work above.

A design modification that could further reduce the likelihood of pin shear failure would be to increase the pin diameter. Increasing the diameter increases the available shear area, reducing the shear stress produced by the same force. A double-shear connection could also provide additional resistance, although this assignment specifically requires the pins to be designed as single-shear connections.

---

## Sources

1. **MEGR 2156/2157 Assignment 2 – Truss Stress**  
   Used for the design constraints, loading conditions, required factors of safety, pin material properties, and CAD requirements.

2. **Steel Tube Institute – ASTM A500**  
   Used as a reference for A500 structural steel material properties.

3. **SolidWorks Material Library**  
   Used for the material properties assigned to the CAD model and the Mass Properties analysis.

---

## AI Use

AI was used as a supporting tool to help explain the truss and pin analysis process, organize the engineering documentation, and provide guidance for creating the SolidWorks model. The calculations, free body diagrams, selected geometry, and CAD model are documented through my own handwritten work and SolidWorks screenshots. AI was used to support the documentation and design process rather than replace the required engineering work.

### Exact AI Prompts and Responses

**[INSERT EXACT AI PROMPTS AND RESPONSES OR SCREENSHOTS HERE]**

