import matplotlib.pyplot as plt
import numpy as np
import math

def fun(x):
  return (x**2)*np.sin(x)
  
x = np.array([0.1, 0.15, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.47, 0.5])
y = np.array([fun(0.1), fun(0.15), fun(0.2), fun(0.3), fun(0.4), fun(0.5), fun(0.6), fun(0.7), fun(0.47), fun(0.5)])
x2= np.array([0.12, 0.152, 0.22, 0.32, 0.42, 0.52, 0.62, 0.72, 0.472, 0.52])
x1 = np.mean(x)
y1 = np.mean(y)
x2 = np.mean(x2)

n=len(x)
num=0
yx=0

for i in range(n):
  num+=x[i]*y[i]
  yx=num/n
  
a1 = (yx-x1*y1)/(x2-x1**2)
a0 = y1-(a1*x1)
print('x =', x1, '\nx2 =', x2, '\ny =', y1, '\nyx =', yx,'\n a1=', a1, '\n a0=', a0)

plt.plot(x, y, 'mo', label='x^2*sin(x)')
plt.plot(x, yx*x+a0, 'b-', label='line approximation')
plt.title('Straight line approximation')
plt.xlabel('x')
plt.ylabel('y')
plt.legend()
plt.show()
