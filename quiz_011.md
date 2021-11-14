```.py

def SameFirstLast(lst):
    lstlen = len(lst)
    if lstlen > 1 and lst[0] == lst[lstlen - 1]:
        tof = "True"
    else:
        tof = "False"
    return tof

output = SameFirstLast([1,2,3])
print(output)

output = SameFirstLast([4,2,4])
print(output)

C:\Users\ASUS\PycharmProjects\pythonProject2\venv\Scripts\python.exe C:/Users/ASUS/PycharmProjects/pythonProject2/main.py
False
True

Process finished with exit code 0



// C++ code
//
void setup()
{
  //code here will run once at the beginning
  //there are no lists in C, only arrays that are fixed so cannot append
  int text_1[3] = {1, 2, 3};
  bool result = SameFirstLast(text_1);
  //communication uses Serial port]
  Serial.begin(9600); //9600 bits per second
  Serial.print("result is: ");
  Serial.println(result);
}

bool SameFirstLast(int list_nums[]){
  //calculate the length of input
  int length = sizeof(list_nums)/sizeof(int);
  //define the variable for the result bool -> True/False
  bool result = false;
  //AND -> &&, OR -> ||, Not -> !
  if (length >= 1 && list_nums[0] == list_nums[length-1])
  {
    result = true;
  }
  return result;
}

void loop()
{
 //Arduino loops here 
}
