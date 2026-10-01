# A6 – [Topic]

## Objective
To Create a CAD Model of A6

## Analyze
Since Stress was governing I used stress values

## Decide
### Bracket Parameters/Desgin

<a href='https://postimages.org/' target='_blank'><img src='https://i.postimg.cc/FK97QhJt/Screenshot-2026-09-30-224056.png' border='0' alt='Screenshot-2026-09-30-224056'></a>
<a href='https://postimages.org/' target='_blank'><img src='https://i.postimg.cc/9fjyw3Rg/A6drwingpic.png' border='0' alt='A6drwingpic'></a>
### Link Parameter/Desgin
<a href='https://postimages.org/' target='_blank'><img src='https://i.postimg.cc/4NPz72vW/actuala6link.png' border='0' alt='actuala6link'></a>
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/pTW8kDBm/A6linktables.png" alt="A6linktables"></a><br><br>
### Files
[A6drwingpic.zip](https://github.com/user-attachments/files/32884137/A6drwingpic.zip)

[A6linkdrwing.zip](https://github.com/user-attachments/files/32884402/A6linkdrwing.zip)
## Communicate
### Overview
There were a few things I did wrong at first like inserting the wrong numbers or symbols for my equations but I got them figured out. Also it was a little tough still figuring out how to use solidworks and its engineering drawing feature.
I spent about 4-5 hours on this assignment. I learned how to add tolerances in Solidworks which is much easier then in Creo. 

### Reflection
a. I drove Feature C's shelf thickness with the stress equation f. In SolidWorks I entered it in the Equations dialog as "t_C", built from other global variables (F, SF, Sy, c_C) instead of a hand-calculated number. The shelf sketch dimension references "t_C". Stress governed at 0.511 in. My calculation changed later: Feature A's stress-required diameter (0.589 in) exceeded my e7 shaft limits, so I moved the cylinder to a 0.625 in nominal and recalculated the RC5 fit.

b. I used a tight tolerance on the Ø0.625 in cylinder (e7, 0.6231 to 0.6238 in) because it is a mating surface. It pivots in the link's H8 hole, and the 0.0012 to 0.0029 in clearance decides whether it turns freely or binds. I used a loose tolerance (X.X, ±.02) on the wall thickness because it is non-critical: it only carries load, and 0.02 in of variation does not affect function. Holding every feature to ±.005 would add reaming, grinding, and inspection steps with no functional benefit, raising cost and scrap, especially in hard-to-machine titanium.

### 2157 Reflection
I tied the link's small hole to the bracket's cylinder diameter, so one change resizes both. Fits must be specified on both mating parts with limits that agree, or the assembled clearance will not match the design. The limit dimensions on the holes, the center-distance tolerance, and the interface note show the machinist which features are critical, while the general block covers the rest.
