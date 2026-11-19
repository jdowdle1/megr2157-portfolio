# A11 – Motor Selection



# A11 – Motor Selection

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

## Downloaded Parts

| Part | McMaster Number | Quantity |
|---|---|---|
| [DC Gearmotor](https://www.mcmaster.com/4855N17) | 4855N17 | 2 |
| [Rigid Coupling](https://www.mcmaster.com/61005K331) | 61005K331 | 2 |
| [T-Slot Framing](https://www.mcmaster.com/5537T912) | 5537T912 | As needed |
| [ACME Leadscrew](https://www.mcmaster.com/99030A030) | 99030A030 | 2 |
| [Bronze Flange Nut](https://www.mcmaster.com/97790A140) | 97790A140 | 2 |


### Draft SolidWorks CAD Files

**DRAFT Motor Mount (Designed in SolidWorks)**

[Download Motor Mount](leadframedesign/Motor%20mount.SLDPRT)

**DRAFT Tensile Tester Assembly (Pack and Go)**

[Download Assembly](leadframedesign/leadframedesign.SLDASM)


## 5. FEA Test 1

### Mesh
<a href="https://postimg.cc/fJyQS18v" target="_blank"><img src="https://i.postimg.cc/CLHhXgD9/A11-mesh.png" alt="A11-mesh"></a><br><br>
### Stress
<a href="https://postimg.cc/PP7sWK7Z" target="_blank"><img src="https://i.postimg.cc/T3ddX4qk/A11-stress.png" alt="A11-stress"></a><br><br>
### Displacement
<a href="https://postimg.cc/KRjh3C0P" target="_blank"><img src="https://i.postimg.cc/ncYFgJ7P/A11-displacement.png" alt="A11-displacement"></a><br><br>
### Safety Factor
<a href="https://postimg.cc/ZCQt8jQN" target="_blank"><img src="https://i.postimg.cc/W1NNPH65/A11-safetyfactor.png" alt="A11-safetyfactor"></a><br><br>

### Improvements
From the images above I saw that the bar is internally too weak. The thickness of the bar is the first thing that needs to be improved. It's only around 8 mm, which is way too thin to support the 1 kN load on both of the lead screw holes. After finding the proper thickness, it would then be best if there was a way to cut out some weight to optimize the design. 

## 6. FEA Test 2

### Mesh
<a href='https://postimg.cc/fJbQ0kw7' target='_blank'><img src='https://i.postimg.cc/gkVzQ6Q7/A11-mesh2.png' border='0' alt='A11-mesh2'></a>
### Stress
<a href="https://postimg.cc/w1hyyWxL" target="_blank"><img src="https://i.postimg.cc/3xqgq6PS/A11-2astress.png" alt="A11-2astress"></a><br><br>
### Displacement
<a href="https://postimg.cc/cvQggD1k" target="_blank"><img src="https://i.postimg.cc/nhWvW5yx/A11-2disp.png" alt="A11-2disp"></a><br><br>
### Safety Factor
<a href="https://postimg.cc/qt4t88g8" target="_blank"><img src="https://i.postimg.cc/HL7Q1zgP/A11-2stress.png" alt="A11-2stress"></a><br><br>

### Improvements
There might be improvements like increasing the thickness of our material, but we are constrained a little by the requirements of the assignment. I believe it is pretty well designed based on all of the parameters.

## 7. Bearing Design 

### Bearing Design 
<a href='https://postimages.org/' target='_blank'><img src='https://i.postimg.cc/4xzTmksL/A11-pt7.png' border='0' alt='A11-pt7'></a>




## 8. Bill of Materials


| Item Number | Quantity | Name | Cost/Item | Cost | Purchase Link |
| --- | --- | --- | --- | --- | --- |
| 1 | 2 | Flange nut | $201.69 | $403.38 | [Flange Nut](https://www.mcmaster.com/97790A140/) |
| 2 | 2 | Lead Screw | $76 | $152.36 | [Lead Screw](https://www.mcmaster.com/99030A030/) |
| 3 | 1 | Cross head material | $75 | $74.94 | [Cross head Material](https://www.mcmaster.com/8910K37-9143K544/) |
| 4 | 8 | Flange nut bolt | $0.36 | $2.88 | [Flange-nut Bolts](https://www.mcmaster.com/92865A589/) |
| 5 | 8 | Flange nut nuts | $0.09 | $0.72 | [Flange-nut Nuts](https://www.mcmaster.com/94846A030/) |
| 6 | 2 | Shaft Clamp | $45.93 | $91.86 | [Shaft Clamp](https://www.mcmaster.com/61005K331/) |
| 7 | 8 | Corner Bracket | $6.44 | $51.52 | [Corner Bracket](https://www.mcmaster.com/5537T935/) |
| 8 | 2 | DC Motor | $575.30 | $1150.60 | [DC Motor](https://www.mcmaster.com/4855N17/) |
| 9 | 2 | T-Slot Framing | $17.28 | $34.56 | [T-Slot Framing](https://www.mcmaster.com/5537T912/) |

 **Total Cost**  **$2112.70**

### Design Cost

| Person | Hours worked | Cost/Hour | Cost |
| --- | --- | --- | --- |
| Dillon B | 9 | $35 | $315 |
| Ameer A | 13 | $35 | $455 |
| Jackson D | 8 | $35 | $280 |
| **Total Cost** | | | **$1050.00** |

**Total Cost of Project:** **$3162.70**



## 9. Lessons Learned

(Ameer A) I learned how to select a motor using torque and speed requirements, calculate bearing stress for a motor mount, and analyze torsional shear stress in a coupling. I also learned how important accurate mounting-hole dimensions are when assembling downloaded parts in SolidWorks. Initially, I designed the motor mount with separate standoffs. I later changed it to one long mounting plate to support both motors. I also had trouble aligning the motor shafts with the leadscrews because the motor mounting holes were offset from the shaft center. I corrected the mounting-hole positions and checked them in SolidWorks. Another issue was that the motor shafts and leadscrews had different diameters, requiring a modified shaft connection.

(Dillon B) Throughout this assignment I have learned the importance of working as a team and communicating the end goal of a project with others. It is important to be on the same page before and especially during the span of the project. A small mistake of one person can affect the entire project and takes excess time to correct. 

## 2157 Portion

The bill of materials for this section was integrated into section 8 bill of materials.


### Drawings
#### Designed Parts
Motor Mount (Pack and Go)
[MotorMount.zip](https://github.com/user-attachments/files/35063150/MM2.0.zip)
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/D0m7VkP1/Screenshot-2026-11-18-213207.png" alt="Screenshot-2026-11-18-213207"></a><br><br>

Crosshead (Pack and Go)
[crosshead.zip](https://github.com/user-attachments/files/35063203/crossheadFEA.zip)
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/nrMn8bG2/Screenshot-2026-11-18-214854.png" alt="Screenshot-2026-11-18-214854"></a><br><br>


Base (Pack and Go)
[Base.zip](https://github.com/user-attachments/files/35063358/basetop.zip)
<a href="https://postimg.cc/xNrwHZ7J" target="_blank"><img src="https://i.postimg.cc/hvhKFW1r/Screenshot-2026-11-18-214631.png" alt="Screenshot-2026-11-18-214631"></a><br><br>



#### Isometric view of frame
<a href='https://postimages.org/' target='_blank'><img src='https://i.postimg.cc/MGpvt4jv/Screenshot-2026-11-18-223319.png' border='0' alt='Screenshot-2026-11-18-223319'></a>


## Final CAD Files
Due to githubs file size constraints, the motor was removed from the assembly. Linked below is the assembly and motor separately for download.

[4855N17_DC Gearmotor.zip](https://github.com/user-attachments/files/35065019/4855N17_DC.Gearmotor.zip)



[leadframedesign.zip](https://github.com/user-attachments/files/35065018/leadframedesign.zip)



