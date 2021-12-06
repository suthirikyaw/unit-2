```.py

def mirrorTime(n):
    if n<=12:
        time1 = str(n) + ':' + str(n)

        tens = int(n/10)
        ones = int(abs((n-(tens*10))))

        time2 = str(n) + ':' + str(ones) + str(tens)

    else:
        return 'None'

    return time1, time2

output = mirrorTime(11)
print(output)

output = mirrorTime(12)
print(output)

C:\Users\ASUS\PycharmProjects\pythonProject2\venv\Scripts\python.exe C:/Users/ASUS/PycharmProjects/pythonProject2/main.py
('11:11', '11:11')
('12:12', '12:21')

Process finished with exit code 0
