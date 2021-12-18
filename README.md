# Math-library
#display sqrt() and cbrt() of the number entered by the user
#include <iostream>
#include<math.h>
using namespace std;
int main()
{
	int number;    //declaring variable 'number' with datatype integer
	cout << "Enter a number: ";
	cin >> number;
	while (cin.fail() != 0)  //if user enters any other character except for number then it will ask the user to enter the number again
	{
		cout << "\aInvalid command! \nEnter the number again: ";
		cin.clear();
		cin.ignore();
		cin >> number;   //the user input will be stored in the variable 'number' using cin function
	}

	cout << "The square root of " << number << " is " << sqrt(number) << endl; //square root of that number will be displayed on the console screen

	cout << "The cube root of " << number << " is " << cbrt(number) << endl;  //cube root of that number will be displayed on the console screen



	return 0;
}
