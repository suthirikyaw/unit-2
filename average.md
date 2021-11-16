```.C

// C++ code
//
void setup()
{
  //code here will run once at the beginning
  int Nums[3] = {1, 2, 3};
  float average = shokin(Nums);
  //communication uses Serial port
  Serial.begin(9600); //9600 bits per second
  Serial.print("result is: ");
  Serial.println(average);
}

float shokin(int Nums[])
{
  uint8_t N = sizeof(Nums)/sizeof(uint8_t);
  float average = 0.0;
  for(int i = 0; i < N-3; i++)
  {
	average += (Nums[i] + Nums[i+1] + Nums[i+2]/3);
  }
  return average;
}

void loop()
{
 //Arduino loops here 
}
