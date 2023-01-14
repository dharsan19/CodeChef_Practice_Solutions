# Overspeeding Fine
## Problem
Chef was driving on a highway at a speed of XX km/hour.

To avoid accidents, there are fine imposed on overspeeding as follows:

No fine if the speed of the car \leq 70≤70 km/hour.
Rs 500500 fine if the speed of the car is strictly greater than 7070 and \leq 100≤100.
Rs 20002000 fine if the speed of the car is strictly greater than 100100.
Determine the fine Chef needs to pay.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of a single integer XX denoting the speed of Chef's car.
## Output Format
For each test case, output the fine paid by Chef.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int speed;
	    cin>>speed;
	    if(speed<=70)
	    {
	        cout<<0<<endl;
	    }
	    else if((speed>70) && (speed<=100))
	    {
	        cout<<500<<endl;
	    }
	    else
	    {
	        cout<<2000<<endl;
	    }
	}
	return 0;
}

```