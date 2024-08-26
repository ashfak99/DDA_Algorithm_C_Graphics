# DDA_Algorithm_C_Graphics
The Digital Differential Analyzer (DDA) ia a scan-conversion line algorithm based on calculating either delta_y(△y) or delta_x(△x)<br><br>
using following equation<br><br>
△y=m.△x      ...(1)<br><br>
△x=△y/m      ...(2)<br><br>
We sample the line at unit intervals in one co-ordinates and determine corresponding integer values nearest the line path for the other co-ordinate.<br><br>
Consider first a line with positive m,<br><br>
If m<=1<br><br>
△x=1<br><br>
y<sub>k+1</sub>=y<sub>k</sub>+m    ....(3)<br><br>
k ∈ 1 -> endpoint<br><br>
m ∈ R (0,1)<br><br>
Calculate y values must be rounded to the nearest integer<br><br>
For line with positive(+ve) m>1<br><br>
△y=1<br><br>
x<sub>k+1</sub>=x<sub>k</sub>+1/m    .....(4)<br><br>
Equation 3 and 4 are based on the assumption that lines are to be processed from the left endpoint to the right endpoint<br><br>
If this processing is reversed so that the starting endpoint is at the right , then either we have <br><br>
△x=-1<br><br>
y<sub>k+1</sub>=y<sub>k</sub>-m<br><br> ....(5)
m>1   △y=-1<br><br>
x<sub>k+1</sub>=x<sub>k</sub>-1/m<br><br> .....(6)
Equation 3 through 6 can also be used to calculate pixel positions along a line with negative(-ve) m.<br><br>
If abs(m)<1<br><br>
The start endpoint is at the left <br><br>
△x=1<br><br>
calculate y with equation 3<br><br>
the start endpoint is at the right<br><br>
△x=-1<br><br>
calculate y with equation 5<br><br>
If abs(m)<1<br><br>
△y=-1<br><br>
Calculate x with equation 6<br><br>
△y=1<br><br>
Calculate x with equation 4
