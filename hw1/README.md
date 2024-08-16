# Project 1 README

Student: Yuhao Wang (919458549)

## Project Status

"Window/Combinational Analysis" tool of logisim is heavily used in this project. All circuits are thoroughly tested using "Simulate/Test Vector".

### Compare

I use XNOR gates to compare bits. AND-ing XNOR outputs can easily give the equal signal (E). The negative signal (N) is generated as follow: if the highest bit Y2==1 but X2==0, output N set, otherwise if Y2==X2 go on to compare the next bit, so on ...

### Gray

I take down the Gray code column corresponding to my SID last digit (9) and perform combinational analysis on each output bit.

B3 B2 B1 B0 | G3 G2 G1 G0
0 0 0 0 | 0 0 0 1
0 0 0 1 | 0 0 1 1
0 0 1 0 | 0 0 1 0
0 0 1 1 | 0 1 1 0
0 1 0 0 | 0 1 1 1
0 1 0 1 | 0 1 0 1
0 1 1 0 | 0 1 0 0
0 1 1 1 | 1 1 0 0
1 0 0 0 | 1 1 0 1
1 0 0 1 | 1 1 1 1
1 0 1 0 | 1 1 1 0
1 0 1 1 | 1 0 1 0
1 1 0 0 | 1 0 1 1
1 1 0 1 | 1 0 0 1
1 1 1 0 | 1 0 0 0
1 1 1 1 | 0 0 0 0

### FiveSeven

I list the truthtable by hand and perform combinational analysis on each output bit. The truth table is below.

V W X Y Z | A B C D E F G
0 0 0 0 0 | 1 1 1 1 1 1 0
0 0 0 0 1 | 1 0 1 1 0 1 1
0 0 0 1 0 | 0 1 1 0 0 0 0
0 0 0 1 1 | 1 0 1 1 1 1 1
0 0 1 0 0 | 0 1 1 0 0 0 0
0 0 1 0 1 | 1 0 1 1 1 1 1
0 0 1 1 0 | 1 1 0 1 1 0 1
0 0 1 1 1 | 1 1 1 0 0 1 0
0 1 0 0 0 | 0 1 1 0 0 0 0
0 1 0 0 1 | 1 0 1 1 1 1 1
0 1 0 1 0 | 1 1 0 1 1 0 1
0 1 0 1 1 | 1 1 1 0 0 1 0
0 1 1 0 0 | 1 1 0 1 1 0 1
0 1 1 0 1 | 1 1 1 0 0 1 0
0 1 1 1 0 | 1 1 1 1 0 0 1
0 1 1 1 1 | 1 1 1 1 1 1 1
1 0 0 0 0 | 0 1 1 0 0 0 0
1 0 0 0 1 | 1 0 1 1 1 1 1
1 0 0 1 0 | 1 1 0 1 1 0 1
1 0 0 1 1 | 1 1 1 0 0 1 0
1 0 1 0 0 | 1 1 0 1 1 0 1
1 0 1 0 1 | 1 1 1 0 0 1 0
1 0 1 1 0 | 1 1 1 1 0 0 1
1 0 1 1 1 | 1 1 1 1 1 1 1
1 1 0 0 0 | 1 1 0 1 1 0 1
1 1 0 0 1 | 1 1 1 0 0 1 0
1 1 0 1 0 | 1 1 1 1 0 0 1
1 1 0 1 1 | 1 1 1 1 1 1 1
1 1 1 0 0 | 1 1 1 1 0 0 1
1 1 1 0 1 | 1 1 1 1 1 1 1
1 1 1 1 0 | 0 1 1 0 0 1 1
1 1 1 1 1 | 1 1 1 1 0 1 1
