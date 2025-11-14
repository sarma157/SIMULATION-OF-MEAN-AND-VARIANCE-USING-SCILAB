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

vX2=EX2-(EX)^3;
vY2=EY2-(EY)^3;

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
![WhatsApp Image 2025-11-13 at 12 52 29_24b94578](https://github.com/user-attachments/assets/ed9df925-9bee-41d7-9499-74145e5a2502)

![WhatsApp Image 2025-11-13 at 12 52 29_83eb49a3](https://github.com/user-attachments/assets/548ec317-41b0-413f-8d4f-2eb5a93e4ae0)

![WhatsApp Image 2025-11-13 at 12 52 29_baf43c1d](https://github.com/user-attachments/assets/4fc4507d-93f6-473b-ae5d-9b21027948a1)







## OUTPUT



<img width="766" height="720" alt="mean and variance sce op pic" src="https://github.com/user-attachments/assets/333ca54a-247c-4a49-81cf-85366583338c" />



## RESULT:
Thus the mean , variance and cross correlation are executed in Scilab and output is verified.
