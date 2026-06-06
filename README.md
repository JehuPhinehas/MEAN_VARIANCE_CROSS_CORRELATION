# MEAN-VARIANCE-CROSS_CORRELATION-USING-SCILAB
AIM: To write a program for mean, variance and cross correlation in SCILAB and verify the output.

EQUIPMENTS Needed

· Computer with i3 Processor

· SCI LAB

Algorithm

Define the Function: Specify the function you want to simulate. For example, f(x)=sin⁡(x)f(x) = \sin(x)f(x)=sin(x) or any other function.

Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.

Evaluate the Function: Compute the function values at each of these sample points.

Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.

Display Results: Output the computed mean variance and Cross Correlation

PROCEDURE

· Refer Algorithms and write code for the experiment.

· Open SCILAB in System

· Type your code in New Editor

· Save the file

· Execute the code

· If any Error, correct it in code and execute again

· Verify the generated results

PROGRAM
```
clear;
clc;
clear;
function X=f(x)
    z=3*(2-x)^2
    X=x*z
endfunction
a=0;
b=1;
EX=intg(a,b,f);
function Y=c(y)
    z=3*(2-y)^2
    Y=y*z
endfunction
EY=intg(a,b,c);
disp(EX,"i)Mean of X=")
disp(EY,"Mean of Y=")
function X=g(x)
    z=3*(2-x)^2
    X=x^2*z
endfunction
a=0;
b=1;
EX2=intg(a,b,g);
function Y=h(y)
    z=3*(2-y)^2
    Y=y^2*z
endfunction
EY2=intg(a,b,h);
vX2=EX2-(EX)^2;
vY2=EY2-(EY)^2;
disp(vX2,"ii) Variance of X");
disp(vY2,"Variance of Y");
x=[1 3 4 6 7 2 9 8];
y=[2 5 8 4 6 1 7 3];
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);

```
OUTPUT:

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/1125200b-d5eb-4318-a189-e4ce06fff344" />


Cross Correlation

Type in the reference sequence = [1 3 4 6 7 2 9 8]

Type in the second sequence = [2 5 8 4 6 1 7 3]



calculation:

<img width="1015" height="1280" alt="image" src="https://github.com/user-attachments/assets/8a261934-3b11-44b7-9a16-4564dd493cc2" />
<img width="841" height="1280" alt="image" src="https://github.com/user-attachments/assets/a1b31c44-5d5a-4cd7-bcb4-da368a1e5f7b" />
<img width="816" height="1280" alt="image" src="https://github.com/user-attachments/assets/7fb38664-d9d9-43ec-8dae-0ed082ca967c" />
<img width="1600" height="759" alt="image" src="https://github.com/user-attachments/assets/96f2bffb-2df5-41a9-8745-0b47e0f82b14" />




RESULT:

Thus the mean , variance and cross correlation are executed in Scilab and output is verified.
