


```.py
def swap2(str):
    newStr = ""
    for i in range(1, int(len(str)), 2):
        newStr += (str[i]) + (str[i-1])

    return newStr

output = swap2("01ABxy")
print(output)
