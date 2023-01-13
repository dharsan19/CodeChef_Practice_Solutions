# Good Investment or Not
## Problem
Chef has invested his money at an interest rate of XX percent per annum while the current inflation rate is YY percent per annum.

An investment is called good if and only if the interest rate of the investment is at least twice of the inflation rate.
Determine whether the investment made by Chef is good or not.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of two integers XX and YY, the interest rate and the current inflation rate respectively.
## Output Format
For each test case, output YES if the investment is good, NO otherwise.

You can output any letter in any case. For example YES, yes, yES are all considered same.
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
	    if(x>=(y*2))
	    {
	        cout<<"YES"<<endl;
	    }
	    else
	    {
	        cout<<"NO"<<endl;
	    }
	}
	return 0;
}
```