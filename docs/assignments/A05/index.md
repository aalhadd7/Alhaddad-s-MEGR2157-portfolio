# Design Assignment – Bracket and Linkage Analysis

## Design Requirements

The goal of this assignment was to design the bracket shown in the provided project drawings so that it could safely support the required strap load. I selected a design load of 700 lbf and used a safety factor of 4. Aluminum 6061-T6 was used for the design. The bracket was analyzed using both strength and stiffness requirements, with a maximum allowable deflection of 0.005 in.

The bracket was divided into Features A through E. Each feature was analyzed using an appropriate mechanical model, and the reactions from one feature were carried into the next part of the bracket where applicable.

---

## Stress Analysis

For the stress analysis, each feature was analyzed separately using the required free-body diagrams, assumptions, known values, unknown values, equations, and numerical calculations. Feature A was treated as a cantilever beam, Feature B as an axially loaded member, and Feature C as a simply supported beam with a center load. Features D and E were analyzed based on the loads transferred through the bracket.

### Handwritten Stress Analysis


<img width="492" height="645" alt="Screenshot 2026-09-23 at 6 58 26 PM" src="https://github.com/user-attachments/assets/084fea4b-8e38-4f2b-a214-ff4b5923d59c" />





<img width="461" height="604" alt="Screenshot 2026-09-23 at 6 58 46 PM" src="https://github.com/user-attachments/assets/1b447c2e-4aa5-4c09-9645-0d55627a9bba" />




<img width="438" height="578" alt="Screenshot 2026-09-23 at 6 58 59 PM" src="https://github.com/user-attachments/assets/d9758c39-3538-4884-975b-251b456a6f38" />



<img width="466" height="596" alt="Screenshot 2026-09-23 at 6 59 15 PM" src="https://github.com/user-attachments/assets/70b55977-a672-4385-a617-d7dd406ca57e" />



<img width="442" height="254" alt="Screenshot 2026-09-23 at 6 59 29 PM" src="https://github.com/user-attachments/assets/11523eb0-be4c-47f2-8c30-1227f4a44110" />



The minimum dimensions calculated from the stress analysis were approximately:

- Feature A: 1.023 in
- Feature B: 0.070 in
- Feature C: 0.397 in
- Feature D: 0.035 in
- Feature E: 0.324 in

---

## Stiffness Analysis

Each feature was also analyzed using stiffness requirements. The maximum allowable deflection for each feature was limited to 0.005 in. The same general loading models used for the stress analysis were used again, but the dimensions were determined using deformation and beam-deflection equations.

### Handwritten Stiffness Analysis

<img width="436" height="361" alt="Screenshot 2026-09-23 at 7 00 14 PM" src="https://github.com/user-attachments/assets/2f83801a-551e-47e6-890e-e4050b0178dc" />


<img width="513" height="663" alt="Screenshot 2026-09-23 at 7 00 42 PM" src="https://github.com/user-attachments/assets/95ffcadf-4d8d-4771-bad8-ff5ed7bd6eab" />




<img width="485" height="617" alt="Screenshot 2026-09-23 at 7 00 55 PM" src="https://github.com/user-attachments/assets/1167d0da-ac2d-46b5-8b86-5d9cfd5f1936" />





<img width="490" height="378" alt="Screenshot 2026-09-23 at 7 01 10 PM" src="https://github.com/user-attachments/assets/8904c7b0-045b-4912-a932-e64b2368b8a4" />





<img width="399" height="284" alt="Screenshot 2026-09-23 at 7 01 26 PM" src="https://github.com/user-attachments/assets/aad8453d-bb0b-4097-9225-5fc4ca6d3a44" />


The minimum dimensions calculated from the stiffness analysis were approximately:

- Feature A: 0.753 in
- Feature B: 0.014 in
- Feature C: 0.228 in
- Feature D: 0.0053 in
- Feature E: 0.152 in

---

## Multiview Sketches

Two separate multiview sketches were created by hand. The first sketch shows the dimensions obtained from the stress analysis, while the second shows the dimensions obtained from the stiffness analysis.

### Stress-Based Multiview Sketch


<img width="386" height="266" alt="Screenshot 2026-09-23 at 7 01 38 PM" src="https://github.com/user-attachments/assets/6f05c8a7-3f6c-472a-ae95-8613cd8df3f8" />


### Stiffness-Based Multiview Sketch

<img width="381" height="296" alt="Screenshot 2026-09-23 at 7 02 11 PM" src="https://github.com/user-attachments/assets/3a72483d-2396-4d41-bf33-3b1ff3e4882c" />


---

## Lessons Learned

### Governing Failure Mode

The stress and stiffness requirements were compared for each feature to determine which condition controlled the final design. For Feature A, the stress analysis required a minimum diameter of 1.023 in, while the stiffness analysis required 0.753 in. This means that stress governed Feature A by approximately 0.270 in. A similar comparison was made for the other features, and the larger required dimension was used when developing the final design.

### Error Propagation

One important part of this assignment was understanding how an error in one calculation could affect later parts of the design. The forces and reactions calculated for one feature were used as loads for the next feature. For example, the 700-lbf load acting on Feature C produced two 350-lbf support reactions. These reactions were then used when analyzing Features D and E. If the reaction forces were calculated incorrectly, the dimensions calculated for the following features would also be incorrect.

### Assumption Sensitivity

The bracket was assumed to be symmetrically loaded so that the two sides of the bracket carried equal portions of the applied load. Under this assumption, a 700-lbf load produces approximately 350 lbf on each side. If the strap load were shifted away from the center, one side of the bracket could experience a larger load. This would increase the stresses and could require larger dimensions for Features D and E.

---

# 2157 Students Only

## Linkage Design

For the 2157 portion of the assignment, an additional linkage was designed to connect Feature A of the bracket to a 1-in shaft. The linkage was designed using the same 700-lbf applied load, Aluminum 6061-T6, and a safety factor of 4.

The smallest net cross-sectional area around the holes was checked because this represents the critical section of the linkage. Both stress and axial deformation were evaluated.

### Handwritten Linkage Calculations

<img width="434" height="322" alt="Screenshot 2026-09-23 at 7 02 59 PM" src="https://github.com/user-attachments/assets/a1400bc1-2918-4cdd-9d39-a932d2a30afa" />


<img width="498" height="683" alt="Screenshot 2026-09-23 at 7 03 14 PM" src="https://github.com/user-attachments/assets/86500d3f-cb50-42d8-a5df-8c791f07ba69" />


<img width="482" height="595" alt="Screenshot 2026-09-23 at 7 03 24 PM" src="https://github.com/user-attachments/assets/b4065902-49ec-438a-ab38-fc9988e9493a" />



The selected linkage dimensions were approximately:

- Width: 1.50 in
- Thickness: 0.250 in
- Hole center-to-center distance: 3.00 in
- Approximate overall length: 4.50 in

The calculated net-section stress was approximately 7,467 psi, which was below the allowable stress of 10,000 psi. The calculated axial deformation was approximately 0.00224 in, which was also below the maximum allowable deformation of 0.005 in.

---

## Linkage Sketch

A dimensioned hand sketch of the linkage was created showing the Feature A connection, the 1-in shaft connection, width, thickness, hole locations, and center-to-center spacing.

<img width="980" height="469" alt="Screenshot 2026-09-23 at 7 13 31 PM" src="https://github.com/user-attachments/assets/9a15b526-b233-4084-b43e-dac8c109ea94" />

---

## Feature A Fit

The connection at Feature A required a running/sliding fit. A precision running fit was selected so that the linkage could move freely while maintaining a controlled amount of clearance.


---

## Final Design Summary

The final design dimensions were selected by comparing the stress and stiffness results and choosing dimensions that were greater than the calculated minimum requirements.

### Main Bracket

- Material: Aluminum 6061-T6
- Design Load: 700 lbf
- Safety Factor: 4
- Maximum Allowable Deflection: 0.005 in
- Feature A: 1.125 in
- Feature B: 0.125 in
- Feature C: 0.500 in
- Feature D: 0.125 in
- Feature E: 0.375 in

### 2157 Linkage

- Material: Aluminum 6061-T6
- Width: 1.50 in
- Thickness: 0.250 in
- Hole Center-to-Center Distance: 3.00 in
- Approximate Overall Length: 4.50 in
- Feature A Connection: Running/Sliding Fit
- 1-in Shaft Connection: Light-Pressure Interference Fit

The final dimensions were rounded upward from the calculated minimum values so the finished design would satisfy both the strength and stiffness requirements.
