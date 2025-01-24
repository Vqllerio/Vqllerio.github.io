---
title: "Systems of Linear Equations"
layout: post
date: "2025-01-03 00:00:00 +0800"
categories: [Linear Algebra]
tags: [Math]
image:
    path: /assets/images/Linear_Algebra.png
---
### One Variable Equation
This is the simplest case where there’s only one unknown variable, like 
𝑥
x.

Example:
```
2𝑥 + 5 = 15
```

## Steps to Solve:
* Isolate 𝑥 by moving constants to the other side:
```
2𝑥 = 15 − 5
2𝑥 = 10
```
* Divide by the coefficient of 
```
𝑥 = 10 / 2
𝑥 = 5
```
* Two Variable Equations (Systems of Linear Equations)
When there are two variables (like 𝑥 and 𝑦), we need two equations to solve them.

Example:
```
𝑥 + 𝑦 = 7
2𝑥 − 𝑦 = 3
```

### Methods to Solve:

## Substitution Method
Solve one equation for one variable, then substitute it into the other equation.

From 
𝑥 + 𝑦 = 7, solve for 𝑦

𝑦 = 7 − 𝑥
Substitute 
𝑦
=
7
−
𝑥
y=7−x into 
2
𝑥
−
𝑦
=
3
2x−y=3:
2
𝑥
−
(
7
−
𝑥
)
=
3
2x−(7−x)=3
2
𝑥
−
7
+
𝑥
=
3
2x−7+x=3
3
𝑥
=
10
  
⟹
  
𝑥
=
10
3
3x=10⟹x= 
3
10
​
 
Use 
𝑥
=
10
3
x= 
3
10
​
  in 
𝑦
=
7
−
𝑥
y=7−x to find 
𝑦
y.
Elimination Method
Add or subtract the equations to eliminate one variable.

Add the equations:
𝑥
+
𝑦
+
2
𝑥
−
𝑦
=
7
+
3
x+y+2x−y=7+3
3
𝑥
=
10
  
⟹
  
𝑥
=
10
3
3x=10⟹x= 
3
10
​
 
3 Variable Equations (Systems of Linear Equations)
When there are three variables (like 
𝑥
x, 
𝑦
y, 
𝑧
z), we need three equations.

Example:

𝑥
+
𝑦
+
𝑧
=
6
2
𝑥
−
𝑦
+
3
𝑧
=
14
3
𝑥
+
2
𝑦
−
𝑧
=
10
x+y+z
2x−y+3z
3x+2y−z
​
  
=6
=14
=10
​
 
Steps to Solve:

Eliminate One Variable
Use two pairs of equations to eliminate one variable.

From 
𝑥
+
𝑦
+
𝑧
=
6
x+y+z=6 and 
2
𝑥
−
𝑦
+
3
𝑧
=
14
2x−y+3z=14, eliminate 
𝑦
y: Multiply 
𝑥
+
𝑦
+
𝑧
=
6
x+y+z=6 by 2:
2
𝑥
+
2
𝑦
+
2
𝑧
=
12
2x+2y+2z=12
Subtract 
2
𝑥
−
𝑦
+
3
𝑧
=
14
2x−y+3z=14:
(
2
𝑥
+
2
𝑦
+
2
𝑧
)
−
(
2
𝑥
−
𝑦
+
3
𝑧
)
=
12
−
14
(2x+2y+2z)−(2x−y+3z)=12−14
3
𝑦
−
𝑧
=
−
2
(Equation 4)
3y−z=−2(Equation 4)
Reduce to Two Variables
Repeat with a different pair of equations to get another equation with two variables.

Solve the Two-Variable System
Use substitution or elimination to solve the reduced system, then back-substitute to find the third variable.