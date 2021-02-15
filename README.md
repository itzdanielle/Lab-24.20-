# Lab-24.20-
#include <iostream>
using namespace std;

double findHighTemp (int temperature[], int& numberOfTemp) {
  int max;
  max = temperature[0];
  for (int i = 0; i < numberOfTemp; i++) {
    if (temperature [i] > max)
    max = temperature[i];
  }
  cout << "The highest temperature is " << max << endl;
  return max;
}
double findLowTemp (int temperature[], int& numberOfTemp) {
  int min;
min = temperature[0];
for (int i = 0; i < numberOfTemp; i++) {
    if (temperature [i] < min)
    min = temperature[i];
  }
  cout << "The lowest temperature is " << min << endl;
  return min;
}
double findAverage (int temperature [], int& numberOfTemp) {
  int sum, i;
  sum += temperature [i];
  double average = sum/numberOfTemp;
  cout << "The average temperature is " << average << endl;
  return average;
}

int main() {
const int MAX_TEMP = 50;
int temperatures [MAX_TEMP];
int i, temperature [i], max, min;
int numberOfTemp;
double average; 
cout << "Enter the temperatures to be read" << endl;
cin >> numberOfTemp;
cout << "Enter a temperature 1 - 100: "<< endl;
cin >> temperature[i];
for (i = 0; i < numberOfTemp; i++) {
cin >> temperature[i];
}
findHighTemp(temperature,numberOfTemp);
findLowTemp(temperature,numberOfTemp);
findAverage(temperature,numberOfTemp); 
}
