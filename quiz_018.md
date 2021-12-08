```.py

def sum67(nums):
    numSix = 0
    numSeven = 0
    numsLen = len(nums)
    sum = 0

    if 6 in nums:
        for i in range(numsLen):
            if nums[i] == 6:
                numSix = i

            elif nums[i] == 7:
                numSeven = i

        for j in range(0, numSix):
            sum += nums[j]

        for j in range(numSeven + 1, numsLen):
            sum += nums[j]

    if not 6 in nums:
        for i in range(len(nums)):
            sum += nums[i]

    return sum

output = sum67([1,1,1,1,6,1,1,1,1,7,1,1,1])
print(output)

output = sum67([1,1,1,1,6,1,1,1,1,1,1,7,1,1])
print(output)

C:\Users\ASUS\PycharmProjects\pythonProject2\venv\Scripts\python.exe C:/Users/ASUS/PycharmProjects/pythonProject2/main.py
7
6

Process finished with exit code 0
