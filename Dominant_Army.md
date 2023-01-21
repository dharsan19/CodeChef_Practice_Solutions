# Dominant Army
## Problem
In the medieval age, there were 3 kingdoms A, B, and C. The army of these kingdom had NA, NB, and NC soldiers respectively.

You are given that an army with X soldiers can defeat an army with Y soldiers only if >X>Y.

An army is said to be dominant if it can defeat both the other armies combined. For example, kingdom C's army will be dominant only if NC >NA+NB.

Determine whether any of the armies is dominant or not.

## Input Format
The first line contains a single integer T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains three integers NA, NB, and NC - the number of warriors in the armies of kingdoms A, B, and C respectively.
## Output Format
For each test case, output YES if any of the armies is dominant. Otherwise, output NO.

You may print each character of YES and NO in uppercase or lowercase (for example, yes, yEs, Yes will be considered identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n1,n2,n3;
	    cin>>n1>>n2>>n3;
	    if(n1 > n2+n3)
	    {
	        cout<<"Yes"<<endl;
	    }
	    else if(n2 > n1+n3)
	    {
	        cout<<"Yes"<<endl;
	    }
	    else if(n3 > n1+n2)
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