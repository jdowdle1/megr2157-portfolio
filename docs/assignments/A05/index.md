# A5 – [Topic]

## Objective
Make a beam in the shape of a T to support a strap

## Analyze
Design the bracket with my own dimension and use stress and stiffness analysis to help.
## Decide
### Stress Analysis
#### Feature A
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/vZCHV8Xv/A5-Astress.png" alt="A5-Astress"></a><br><br>
#### Feature B and C
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/q7nBXfZ8/A5BCstress.png" alt="A5BCstress"></a><br><br>
#### Feature D and E
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/5tv9qck5/A5DEstress.png" alt="A5DEstress"></a><br><br>
### Stiffness Analysis
#### Feature A, B, and C
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/GhHCxw4s/A5stiffabc.png" alt="A5stiffabc"></a><br><br>
#### Feature D and E
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/pXpHJbmF/A5stiffde.png" alt="A5stiffde"></a><br><br>
#### Comparison Table
<a href='https://postimages.org/' target='_blank'><img src='https://i.postimg.cc/XNDMJHsf/Stressvs-Stifftable.png' border='0' alt='Stressvs-Stifftable'></a>

It is clear the stress governed every feature.
### Stress Iso View
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/7Yfkn857/A5Stressiso.png" alt="A5Stressiso"></a><br><br>
### Stiffness Iso View
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/L6np3KJL/A5stiffiso.png" alt="A5stiffiso"></a><br><br>
### MEGR 2157 Students Only
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/wT7pQ81N/A52157only.png" alt="A52157only"></a><br><br>

## Communicate
### Governing Failure Mode
Stress governed all five features. Feature A had the largest margin, while Feature B had the smallest margin. Feature C was the next closest to its required size.
### Error Propagation
The 800 lbf load applies to Features A and B individually. Features C, D, and E must handle the combined 1,600 lbf load. Using 800 lbf for C, D, and E would make their required dimensions too small.
### Assumption Sensitivity
The most important assumptions are the loads on each feature, the lever-arm lengths, and the width. Errors in these values would directly affect the final dimensions. The final CAD design should be checked to confirm these assumptions.
