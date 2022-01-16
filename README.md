# Code-1


#include <iostream>
#include <string>
using namespace std;

int main()
{
	int age;
	cout << "Enter your age :\n Age limit is 16 - 30" << endl;
	cin >> age;
	while (cin.fail())
	{
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Incorrect command, enter the age again:\nLimit is 16 - 30 " << endl;
		cin >> age;
	}

	if (age >= 16 && age <= 21 )
	{
		string ans;
		cout << "Do you want to go to the Mall?\n Type Y for Yes\n  Type N for No " << endl;
		cin >> ans;
		if (ans == "y" || ans == "Y")
		{
			cout << "Enjoy" << endl;
		}
		else if (ans == "n" || ans == "N")
		{
			cout << "Cancelled" << endl;
		}
		else {
			cout << "Incorrect command!" << endl;
		}
	}
	if (age >= 22 && age <= 30)
	{
		string input;
		cout << "Would you like to go to a trip to Hawaii?\n Type Y for yes \n Type N for No" << endl;
		cin >> input;
		if (input == "y" || input == "Y")
		{
			cout << "Enjoy" << endl;
		}
		else if (input == "n" || input == "N")
		{
			cout << "Cancelled" << endl;
		}
		else {
			cout << "Incorrect command!" << endl;
		}
	}
	else
	{
		cout << "Incorrect command!" << endl;
	}

	return 0;
}
