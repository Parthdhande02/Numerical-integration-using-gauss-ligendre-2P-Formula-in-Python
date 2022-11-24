# Numerical-integration-using-gauss-ligendre-2P-Formula-in-Python

import math


def f(x):
    return math.exp(-x/2)


x0 = int(input("Enter the value of lower limit"))
xn = int(input("Enter the value of upper limit"))
c = (xn-x0)/2
d = (xn+x0)/2

x1 = (c/math.sqrt(3)) + d
x2 = (-c/math.sqrt(3)) + d

y1 = f(x1)
y2 = f(x2)

solution = (y1+y2)*c
print(solution)
