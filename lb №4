from numpy import linalg
import numpy as np

print ("TASK 1")
a = np.matrix([[2,3,1],[-1,1,0],[1,2,-1]])
b = np.matrix ([[1,2,1],[0,1,2],[3,1,1]])
solve = (a*b)-(b*a)
print ("Matrix:\n", solve)


print ("\nTASK 2")
c = np.matrix ([[-1,0,2],[0, 1, 0], [1, 2, -1]])
print ("Matrix power:\n", c**2 )


print ("\nTASK 3")
d = np.matrix ([[5,8,-4],[6, 9, -5], [4, 7, -3]])
i = np.matrix ([[3,2,5],[4, -1, 3], [9, 6, 5]])
print ("Product matrix:\n", d*i )


print ("\nTASK 4")
f = np.linalg.det ([[1,5,-5],[4,0,3],[2,-10,3]])
print ("Determinants:\n", f)


print ("\nTASK 5")
e = np.linalg.det ([[1,2,0,0,0],[1,0,2,0,0],[1,0,0,2,0],[1,0,0,0,2],[0,0,1,1,1]])
print ("Determinants:\n", e)


print ("\nTASK 6")
j = np.linalg.inv ([[1,2,-3],[0, 1, 2], [0, 0, 1]])
print ("Inverse matrix:\n", j)


print ("\nTASK 7")
k = np.linalg.matrix_rank ([[-2,3,1,-1],[3,2,1,4],[1,2,3,4],[0,2,3,3]])
print ("Rank matrix:", k)


print ("\nTASK 8")
def kramer():
    l=np.matrix([[14,4,6],[5,-3,2],[10,-11,5]])
    m=np.matrix([[30],[15],[36]])
    l_det=np.linalg.det(l)
    if l_det != 0:
        x_n=np.matrix(l)
        x_n[:,0]=m
        y_n=np.matrix(l)
        y_n[:,1]=m
        z_n=np.matrix(l)
        z_n[:,2]=m
    
        x=np.linalg.det(x_n)/l_det
        y=np.linalg.det(y_n)/l_det
        z=np.linalg.det(z_n)/l_det
        print('Method Kramera:', x, y, z)
        print('Solve:\n', np.linalg.solve(l,m))
    else:
        print('no result')
    return x,y,z
kramer()


print ("\nTASK 9")
def matrix():
    o=np.matrix('4,1,4;1,1,2;2,1,2')
    p=np.matrix('-2;-1;0')
    r=np.linalg.inv(o)
    s = r * p
    print('Matrix method:\n', s)
    print('Solve:\n', np.linalg.solve(o,p))

matrix()


print ("\nTASK 10")
N=4
M=5
A=np.random.randint(1, 100, size=(N,M))
q=np.mean(A, axis=1)
s=np.min(q)
print(A)
print('Arithmetic mean of strings:', q)
print('Minimal arithmetic mean ', s)
