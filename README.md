# DDA_Algorithm_C_Graphics
The Digital Differential Analyzer (DDA) ia a scan-conversion line algorithm based on calculating either delta_y(dy) or delta_x(dx)<br><br>
using following equation<br><br>
dy=m.dx      ...(1)<br><br>
dx=dy/m      ...(2)<br><br>
We sample the line at unit intervals in one co-ordinates and determine corresponding integer values nearest the line path for the other co-ordinate.<br><br>
Consider first a line with positive m,<br><br>
If m<=1<br><br>
dx=1<br><br>
y&#x2082;_(k+1)=y&#x2082;+m   ......(3)<br><br>
y&#x2082;_(k+1)
