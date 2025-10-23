# SIMULATION-OF-MEAN-AND-VARIANCE-USING-SCILAB

## AIM:
To write a program for mean, variance and cross correlation in SCILAB and verify the output.

## EQUIPMENTS Needed

•	Computer with i3 Processor
•	SCI LAB


## Algorithm
1.	Define	the	Function:	Specify the	function	you	want	to	simulate.	For	example, f(x)=sin⁡(x)f(x) = \sin(x)f(x)=sin(x) or any other function.
2.	Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.
3.	Evaluate the Function: Compute the function values at each of these sample points.
4.	Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.
5.	Display Results: Output the computed mean variance and Cross Correlation PROCEDURE
•	Refer Algorithms and write code for the experiment.
•	Open SCILAB in System
•	Type your code in New Editor
•	Save the file
•	Execute the code
•	If any Error, correct it in code and execute again
•	Verify the generated results


## PROGRAM
```
//Mean
function X=f(x)
    z=3*(1-x)^3;
    X=x*z;
endfunction

a=0;
b=1;

EX=intg(a,b,f);
function Y=c(y)
    z=3*(1-y)^3;
    Y=y*z;
endfunction

EY=intg(a,b,c);
disp("i)Mean of X =",EX)
disp("ii) Mean of Y =",EY)

//Variance

function X=g(x)
    z=3*(1-x)^3;
    X=x^2*z;
endfunction

a=0;
b=1;

EX2=intg(a,b,g);
function Y=h(y)
    z=3*(1-y)^3;
    Y=y^2*z;
endfunction

EY2=intg(a,b,h);

vX2=EX2-(EX)^2;
vY2=EY2-(EY)^2;

disp("iii) Variance of X",vX2);
disp("iv) Variance of Y",vY2);

// Cross Correlation

x=input("type in the reference sequence=");
y=input("type in the second sequence=");
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);


```


## CALCULATION
![WhatsApp Image 2025-10-23 at 23 06 46_040cc851](https://github.com/user-attachments/assets/fe68dbfe-aad0-4d0b-85f7-52260be0ab96)
![WhatsApp Image 2025-10-23 at 23 06 46_db2f7e6c](https://github.com/user-attachments/assets/b260c9c1-95ff-4cf3-a1a2-354ca7028c1f)
![WhatsApp Image 2025-10-23 at 23 16 48_9a45a3e9](https://github.com/user-attachments/assets/59965295-23f7-4a0e-bb23-45b1cfc06be0)
![WhatsApp Image 2025-10-23 at 23 16 48_f34b8d46](https://github.com/user-attachments/assets/600c39cc-648d-4d20-9ac0-30847dead6aa)




## OUTPUT

<img width="812" height="410" alt="image" src="https://github.com/user-attachments/assets/1df62304-daf9-4fe1-ade4-cd879f9d1a1b" />


<img width="758" height="721" alt="image" src="https://github.com/user-attachments/assets/1cb1ea40-6ab2-47aa-a9de-94ec111f2bc7" />


## RESULT:
Thus the mean , variance and cross correlation are executed in Scilab and output is verified.
