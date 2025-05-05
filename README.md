import math
x = 0.5
eps = 1e-6 
max_iter = 100
i = 0
while i < max_iter:
    x_next = 0.5 - math.log(x)

    if abs(x_next - x) < eps:
        break
    x = x_next
    i += 1
print("Təqribi kök:", x)
print("İterasiya sayı:", i)
