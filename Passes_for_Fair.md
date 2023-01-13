# Passes for Fair
## Problem
There is a fair going on in Chefland. Chef wants to visit the fair along with his NN friends. Chef manages to collect KK passes for the fair. Will Chef be able to enter the fair with all his NN friends?

A person can enter the fair using one pass, and each pass can be used by only one person.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of a single line containing two space-separated integers N, KN,K.
## Output Format
For each test case, print on a new line YES if Chef will be able to enter the fair with all his NN friends and NO otherwise.

You may print each character of the string in either uppercase or lowercase (for example, the strings yEs, yes, Yes, and YES will all be treated as identical).
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
	    if((a+1)<=b)
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