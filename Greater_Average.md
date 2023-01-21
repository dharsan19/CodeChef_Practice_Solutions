# Greater Average
## Problem
You are given 3 numbers A,B, and C.

Determine whether the average of A and B is strictly greater than C or not?

NOTE: Average of A and B is defined as (A+B)/2. For example, average of 5 and 9 is 7, average of 5 and 8 is 6.5.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of 3 integers A,B, and C.
## Output Format
For each test case, output YES if average of A and B is strictly greater than C, NO otherwise.

You may print each character of the string in uppercase or lowercase (for example, the strings YeS, yEs, yes and YES will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    float a,b,c;
	    cin>>a>>b>>c;
	    if((a+b)/2 > c)
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