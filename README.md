###### -6666666




#include <iostream>
using namespace std;

int main()
{
  const int NUMBER_OF_ELEMENTS = 2;
  double numbers[NUMBER_OF_ELEMENTS];
  double numbers_squared[NUMBER_OF_ELEMENTS];
  double sum = 0;

  for (int i = 0; i < NUMBER_OF_ELEMENTS; i++)
  {
    cout << "請輸入一個數: ";
    cin >> numbers[i];
    sum += numbers[i];
    numbers_squared[1]=numbers[1]*numbers[1];
  }
    
    cout << "numbers[1] is " << numbers[1] << endl;
    cout << "numbers_squared[1] is " << numbers_squared[1] << endl;
    double average = sum / NUMBER_OF_ELEMENTS;

  int count = 0; // The number of elements above average
  for (int i = 0; i < NUMBER_OF_ELEMENTS; i++)
    if (numbers[i] > average)
      count++;

  cout << "平均是 " << average << endl;
  cout << "高於平均值的元素數量 " << count << endl;
     system("pause");
  return 0;
}
