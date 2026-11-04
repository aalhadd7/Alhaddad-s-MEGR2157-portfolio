# Assignment 8: Pulley System

## Project Overview

For this assignment, I worked on designing a pulley system that transfers power between two parallel shafts. The purpose was to use engineering calculations to determine the belt size, shaft diameter, journal bearing requirements, and frame strength. The system consists of two 3-inch pulleys separated by a center distance of 5 inches. I selected an operating speed of 1500 rpm and a static belt tension of 5 lbf. The design also needed to meet a minimum safety factor of 3.

## Part 1: Belt Design

I started by identifying the known and unknown values for the pulley system. I used the selected operating conditions to calculate the tight-side and loose-side belt tensions. Using an assumed driving force of 3 lbf, I calculated a tight-side tension of 6.5 lbf and a loose-side tension of 3.5 lbf. I then checked the friction condition to determine whether the belt would slip. Using the normal stress equation and the polyurethane rubber yield strength, I calculated a minimum belt diameter of approximately 0.230 inches. I selected a 0.250-inch belt and calculated an approximate installed belt length of 20.21 inches.

**Handwritten Calculations and Free-Body Diagram**

<img width="677" height="861" alt="Screenshot 2026-11-04 at 6 56 57 PM" src="https://github.com/user-attachments/assets/f97e7b29-e4d7-4743-a032-496188cf7ff5" />

## Part 2: Shaft Design

Next, I calculated the minimum shaft diameter needed to withstand the torque produced by the pulley system. The shaft material was 1060 hardened steel. Using the difference between the tight-side and loose-side tensions and the pulley radius, I calculated a torque of 4.5 lbf-in. I then used the torsional shear stress equation and an assumed yield strength of 70,000 psi to determine the minimum shaft diameter. The calculated diameter was approximately 0.119 inches, and I selected a shaft diameter of 0.375 inches. This provided a larger diameter than the calculated torsional minimum.

**Handwritten Calculations and Free-Body Diagram**

<img width="620" height="663" alt="Screenshot 2026-11-04 at 6 57 35 PM" src="https://github.com/user-attachments/assets/63211e4d-6c17-4e70-8949-7058a7c3ac77" />

## Part 3: Journal Bearing Design

For the journal bearing design, I calculated the radial load, bearing pressure, linear velocity, and PV rating. Using the belt tensions, I calculated a radial load of 10 lbf. I used a shaft diameter of 0.375 inches and a selected bearing length of 0.50 inches. The bearing pressure was calculated to be 53.33 psi, while the linear velocity was 147.26 ft/min. Using these values, I calculated a PV rating of approximately 7,854 psi-ft/min. I identified oil-impregnated sintered bronze as a possible bearing material, although its rated limits would still need to be verified.

**Handwritten Calculations and Free-Body Diagram**

<img width="678" height="824" alt="Screenshot 2026-11-04 at 6 57 58 PM" src="https://github.com/user-attachments/assets/8a146de7-a68f-4eb2-91f7-fa51b5a5b70e" />

## Part 4: Frame Design

For the frame design, I used the A-frame concept provided in the assignment as a reference. The frame was intended to support the two pulley shafts while maintaining the required 5-inch center distance. I selected aluminum 6061-T6 as the frame material and used preliminary dimensions of 6.5 inches in length, 1 inch in width, and 0.25 inches in thickness. Using a simplified compressive load of 10 lbf, I calculated a compressive stress of 40 psi and a safety factor of 875. I also calculated the net-sectional area around the shaft hole, which resulted in a net-section stress of 64 psi and a safety factor of approximately 546.88. Finally, I evaluated the frame for buckling and calculated a theoretical critical buckling load of approximately 5,140 lbf, resulting in a buckling safety factor of approximately 514. These preliminary calculations exceeded the minimum required safety factor of 3 under the assumed loading conditions.

**Handwritten Calculations and Free-Body Diagram**

<img width="680" height="850" alt="Screenshot 2026-11-04 at 6 58 20 PM" src="https://github.com/user-attachments/assets/3907ce16-e8ea-4aab-adc9-277a375a24b1" />

## Part 5: Engineering Lessons Learned

During this assignment, I learned how the forces in a pulley system affect the design of multiple mechanical components. One important concept was understanding how the difference between the tight-side and loose-side belt tensions creates torque. I also learned how friction between the belt and pulley helps prevent slipping during operation. Another important concept I learned was how to calculate the minimum shaft diameter using torsional shear stress. The calculations showed how the shaft diameter depends on the applied torque and the strength of the material. I also learned that selecting a journal bearing requires evaluating both the pressure acting on the bearing and the surface velocity of the rotating shaft. The frame calculations helped me understand how compressive loads can affect a supporting structure. By calculating the stress, safety factor, and critical buckling load, I was able to evaluate the preliminary frame dimensions rather than selecting them based only on appearance. Overall, this assignment helped me understand how belt tension, torque, material strength, and bearing performance are connected. I learned that changing one design parameter can affect the requirements of several other components in the pulley system.

## Time Spent

Total time spent completing the assignment: 5 hours

## Mistakes and Adjustments
One mistake I made during the belt calculations was initially using an assumed driving force of 3 lbf without fully considering how it would affect the rest of the system. I realized that this value was not directly given in the assignment, so I needed to identify it as an assumption. This helped me understand the importance of distinguishing between given values and selected design values when performing engineering calculations.

## Final Documentation

The handwritten engineering calculations and free-body diagrams for all four design sections are included above. These calculations document the process used to develop and evaluate the preliminary pulley system design.

