# Battery Low
## Problem
Chef's phone shows a Battery Low notification if the battery level is 15% or less.

Given that the battery level of Chef's phone is X%, determine whether it would show a Battery low notification.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains a single line of input, an integer X, denoting the battery level of the phone.
## Output Format
For each test case, output in a single line Yes, if the battery level is 15% or below. Otherwise, print No.

You may print each character of Yes and No in uppercase or lowercase (for example, YeS, YES,yes will be considered identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int battery_percent;
	    cin>>battery_percent;
	    if(battery_percent <= 15)
	    {
	        cout<<"Yes"<<endl;
	    }
	    else
	    {
	        cout<<"No"<<endl;
	    }
	}
	return 0;
}
```