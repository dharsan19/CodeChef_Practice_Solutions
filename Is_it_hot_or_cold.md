# Is it hot or cold
## Problem
Chef considers the climate HOT if the temperature is above 20, otherwise he considers it COLD. You are given the temperature C, find whether the climate is HOT or COLD.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
The first and only line of each test case contains a single integer, the temperature C.
## Output Format
For each test case, print on a new line whether the climate is HOT or COLD.

You may print each character of the string in either uppercase or lowercase (for example, the strings hOt, hot, Hot, and HOT will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int temperature;
	    cin>>temperature;
	    if(temperature>20)
	    {
	        cout<<"HOT"<<endl;
	    }
	    else
	    {
	        cout<<"COLD"<<endl;
	    }
	}
	return 0;
}

```