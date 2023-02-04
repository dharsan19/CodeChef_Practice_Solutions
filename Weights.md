# Weights
## Problem
Chef is playing with weights. He has an object weighing W units. He also has three weights each of X,Y, and Z units respectively. Help him determine whether he can measure the exact weight of the object with one or more of these weights.

If it is possible to measure the weight of object with one or more of these weights, print YES, otherwise print NO.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of single line containing a four positive integers W,X,Y, and Z.
## Output Format
For each test case, output on a new line YES if it is possible to measure the weight of object with one or more of these weights, otherwise print NO.

You may print each character of the string in either uppercase or lowercase (for example, the strings yes, YES, Yes, and yeS will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int w,a,b,c;
	    cin>>w>>a>>b>>c;
	    if(w == a || w == b|| w == c|| w == a+b|| w == b+c|| w == c+a || w == a+b+c)
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