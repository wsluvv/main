import math
from numpy import *
import numpy as np
from math import *
from pylab import *
from scipy import integrate


print('1. Мethod of rectangles') 
def calc(a, b, n):
 return (b-a)/float(n)

def rectangles (f, a, b, n):
 er = 0.0001

 dx = calc(a, b, n)
 for i in range (0, n):
         er = er + f((a + (i*dx)))
 return dx*er

def f1(x):
    return 1/(sqrt(0.2*x)+1)
def f2(x):
    return log10(x**2 + 0.8) / (x - 1)         
def f3(x):
    return 1/(sqrt(x**2 + 2))  

print('example 1:', rectangles(f1, 1.3, 2.5, 10))
print('example 2:', rectangles(f2, 2.5, 3.3, 10))
print('example 3:', rectangles(f3, 0.5, 1.3, 10))

print("\n 2.Simpson's method")

def simpson(f, a, b, n):
    if n % 2:
        raise ValueError("n повинно бути парним (отримане n = %d)" % n)

    h = (b - a) / n
    s = f(a) + f(b)

    for i in range(1, n, 2):
        s += 4 * f(a + i * h)
    for i in range(2, n-1, 2):
        s += 2 * f(a + i * h)

    return s * h / 3

print('example 1:', simpson(f1, 1.3, 2.5, 8))
print('example 2:', simpson(f2, 2.5, 3.3, 8))
print('example 3:', simpson(f3, 0.5, 1.3, 8))

print("\n 3.Trapezoidal method")

def Trapezoidal(f, a, b, n):
    d = float(b - a)/(n)
    h = float(b - a) / n
    s = 0.0
    s += f(a)/2.0
    for i in range(1, n):
        s += f(a + i*h)
    s += f(b)/2.0
    return s * h

print('example 1:', Trapezoidal(f1, 1.3, 2.5, 20))
print('example 2:', Trapezoidal(f2, 2.5, 3.3, 20))
print('example 3:', Trapezoidal(f3, 0.5, 1.3, 20))

print('\nСheck')
print('Num1:', integrate.quad(f1, 1.3, 2.5))
print('Num2:', integrate.quad(f2, 2.5, 3.3))
print('Num3:', integrate.quad(f3, 0.5, 1.3))
