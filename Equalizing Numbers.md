# Equalizing Numbers
## Problem
Chef has two integers A and B. In one operation he can choose any integer d, and make one of the following two moves :

Add d to A and subtract d from B.
Add d to B and subtract d from A.
Chef is allowed to make as many operations as he wants. Can he make A and B equal?

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains of a single line of input, two integers A,B.
## Output Format
For each test case, if Chef can make the two numbers equal print YES else print NO.

You may print each character of the string in uppercase or lowercase (for example, the strings yEs, Yes, YeS, and YES will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b;
	    cin>>a>>b;
	    if(((a%2==0) and (b%2 == 0)) or ((a%2 == 1) and (b%2 == 1)))
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