# Bath in Winters
## Problem
A geyser has a capacity of X litres of water and a bucket has a capacity of Y litres of water.

One person requires exactly 2 buckets of water to take a bath. Find the maximum number of people that can take bath using water from one completely filled geyser..

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains a single line of input, two integers X,Y.
## Output Format
For each test case, output the maximum number of people that can take bath.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y;
	    cin>>x>>y;
	    if(x < y)
	    {
	        cout<<0<<endl;
	    }
	    else
	    {
	        cout<<x/(y*2)<<endl;
	    }
	}
	return 0;
}
```