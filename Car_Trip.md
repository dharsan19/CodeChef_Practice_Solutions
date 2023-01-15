# Car Trip
## Problem
Chef rented a car for a day.

Usually, the cost of the car is Rs 1010 per km. However, since Chef has booked the car for the whole day, he needs to pay for at least 300300 kms even if the car runs less than 300300 kms.

If the car ran XX kms, determine the cost Chef needs to pay.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of a single integer XX - denoting the number of kms Chef travelled.
## Output Format
For each test case, output the cost Chef needs to pay.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x;
	    cin>>x;
	    if(x<=300)
	    {
	        cout<<3000<<'\n';
	    }
	    else
	    {
	        cout<<x*10<<'\n';
	    }
	}
	return 0;
}
```