# DDA_Algorithm_C_Graphics
The Digital Differential Analyzer (DDA) ia a scan-conversion line algorithm based on calculating either delta_y(dy) or delta_x(dx)<br>
using following equation<br>
dy=m.dx      ...(1)<br>
dx=dy/m      ...(2)<br>
We sample the line at unit intervals in one co-ordinates and determine corresponding integer values nearest the line path for the other co-ordinate.<br>
Consider first a line with positive m,<br>
If m<=1<br>
dx=1<br>
y&#x2082;k+1
