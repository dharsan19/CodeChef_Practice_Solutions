# Reach on Time
## Problem
Chef has recently moved into an apartment. It takes 3030 minutes for Chef to reach office from the apartment.

Chef left for the office XX minutes before Chef was supposed to reach. Determine whether or not Chef will be able to reach on time.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of a single integer XX.
## Output Format
For each test case, output YES if Chef will reach on time, NO otherwise.

The output is case-insensitive. Thus, the strings YES, yes, yeS, and Yes are all considered the same.
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
	    if(x>=30)
	        cout<<"YES"<<endl;
	    else
	        cout<<"NO"<<endl;
	}
	return 0;
}
```