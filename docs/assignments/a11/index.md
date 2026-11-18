# A11 – Motor Selection and Design

## 1. Motor Selection

For our tensile tester, we needed motors capable of rotating the two leadscrews and producing enough torque to apply the required tensile load.

From our previous calculations:

- Required torque per leadscrew: 1.75 N·m
- Required speed range: 0.39–19.69 RPM
- Safety factor: 4

**Required motor torque:**

I selected two **McMaster-Carr #4855N17 DC gearmotors**.

- Rated torque: 11.30 N·m
- Rated speed: 20 RPM
- Voltage: 90 V DC



The selected motor exceeds the required design torque at its rated operating point. Its rated speed is also close to the maximum required speed. The complete operating speed range still needs verification.

I selected two identical motors so that each motor could operate one leadscrew.

**Part Link:** [McMaster-Carr #4855N17](https://www.mcmaster.com/4855N17)

<img width="528" height="487" alt="Screenshot 2026-11-18 at 6 11 34 PM" src="https://github.com/user-attachments/assets/71bc5355-e025-4433-bc96-3243f84831b8" />

---

## 2. Motor Mount Design

I designed a single aluminum mounting plate to hold both motors at the top of the tensile tester.

The plate dimensions are:

- Length: 330 mm
- Width: 91 mm
- Thickness: 8 mm
- Material: 6061-T6 aluminum
- Distance between motor shafts: 250 mm


The plate passed the preliminary motor bolt bearing-stress calculation.

<img width="460" height="562" alt="Screenshot 2026-11-18 at 6 11 41 PM" src="https://github.com/user-attachments/assets/6e39fb6b-7eee-4e84-8b88-6d26d8cb2279" />

<img width="584" height="316" alt="Unknown" src="https://github.com/user-attachments/assets/613b89a2-ce9f-4cd0-92fb-9a508f4f7499" />

I created the mounting plate in SolidWorks and added two Ø30 mm openings for the motor shafts and eight Ø5.4 mm motor mounting holes.

---

## 3. Coupling Selection

I needed a coupling to connect each motor shaft to its leadscrew.

I selected **McMaster-Carr #61005K331**, a rigid steel clamping coupling.

- Inner diameter: 12.70 mm
- Outer diameter: 28.575 mm
- Length: 44.45 mm
- Rated torque: 107.34 N·m

I chose this coupling because its bore matches the motor shaft and its torque capacity exceeds the motor's rated torque.


The coupling passed the preliminary torsional shear-stress calculation.

The leadscrew end will need to be machined or adapted to fit the coupling.

**Part Link:** [McMaster-Carr #61005K331](https://www.mcmaster.com/61005K331)

<img width="468" height="534" alt="Screenshot 2026-11-18 at 6 11 51 PM" src="https://github.com/user-attachments/assets/ffde878a-6048-46d1-90e3-50276f44c461" />

<img width="452" height="339" alt="Screenshot 2026-11-18 at 6 12 01 PM" src="https://github.com/user-attachments/assets/1a1da1b4-c016-46e3-972e-162268d3acd6" />


<img width="403" height="307" alt="Unknown-1" src="https://github.com/user-attachments/assets/845758d8-5f49-40d7-bfc8-590260327161" />
---

## 4. Top Frame Connections

I used four corner brackets to connect the upper mounting plate to the two vertical T-slot frame members.

I calculated the forces using the maximum tensile load of 2,000 N and the torque of both motors.


<img width="598" height="759" alt="Screenshot 2026-11-18 at 6 06 46 PM" src="https://github.com/user-attachments/assets/c5e15d96-e955-4442-b346-36076af3fdb3" />


<img width="753" height="384" alt="Screenshot 2026-11-18 at 6 07 01 PM" src="https://github.com/user-attachments/assets/d66f4719-03e4-4378-9407-36f762019cde" />


The preliminary required capacity is approximately 2.01 kN per bracket.

I selected 90° gusset brackets because they can connect the upper plate to the vertical T-slot framing.

**Selected bracket:** [McMaster-Carr #5537T658](https://www.mcmaster.com/5537T658)

**T-slot framing:** [McMaster-Carr #5537T912](https://www.mcmaster.com/5537T912)

The bracket load capacity still needs verification.


<img width="516" height="429" alt="Unknown-2" src="https://github.com/user-attachments/assets/c8ad5949-a8f4-48f0-a06b-e022bb5ee010" />
---

## 5. Downloaded Parts

| Part | McMaster Number | Quantity |
|---|---|---|
| [DC Gearmotor](https://www.mcmaster.com/4855N17) | 4855N17 | 2 |
| [Rigid Coupling](https://www.mcmaster.com/61005K331) | 61005K331 | 2 |
| [Corner Bracket](https://www.mcmaster.com/5537T658) | 5537T658 | 4 |
| [T-Slot Framing](https://www.mcmaster.com/5537T912) | 5537T912 | As needed |
| [ACME Leadscrew](https://www.mcmaster.com/99030A030) | 99030A030 | 2 |
| [Bronze Flange Nut](https://www.mcmaster.com/97790A140) | 97790A140 | 2 |


### SolidWorks CAD Files

**Motor Mount (Designed in SolidWorks)**

[Download Motor Mount](leadframedesign/Motor%20mount.SLDPRT)

**Complete Tensile Tester Assembly (Pack and Go)**

[Download Complete Assembly](leadframedesign/leadframedesign.SLDASM)


---

## 6. Problems and Changes

Initially, I designed the motor mount with separate standoffs. I later changed it to one long mounting plate to support both motors. I also had trouble aligning the motor shafts with the leadscrews because the motor mounting holes were offset from the shaft center. I corrected the mounting-hole positions and checked them in SolidWorks. Another issue was that the motor shafts and leadscrews had different diameters, requiring a modified shaft connection.

## 7. Lessons Learned

I learned how to select a motor using torque and speed requirements, calculate bearing stress for a motor mount, and analyze torsional shear stress in a coupling. I also learned how important accurate mounting-hole dimensions are when assembling downloaded parts in SolidWorks.

**Time Spent:** 8 hours
