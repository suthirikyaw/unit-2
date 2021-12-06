






```.py

def triangle(a, b, c):
    if a+b>c and a+c>b and b+c>a:
        tof = "TRUE"
    else:
        tof = "FALSE"

    return tof

output = triangle(1,1,2)
print(output)

output = triangle(5,6,3)
print(output)

output = triangle(1,2,9)
print(output)
