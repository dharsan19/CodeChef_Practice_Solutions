# Make AP
## Problem
Chef is given two integers A and C such that A≤C.

Chef wants to find whether there exists any integer B such that A,B, and C are in arithmetic progression.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of two space-separated integers A and C, the given integers.
## Output Format
For each test case, output −1 if there exists no integer B such that A,B, and C are in arithmetic progression. Else, output the value of B.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b = -1,c;
	    cin>>a>>c;
	    for(int i = a; i < c;i++)
	    {
	        if(i-a == c-i)
	        {
	            b = i;
	            break;
	        }
	        
	    }
	    if( a == c)
	    {
	        cout<<a<<endl;
	    }
	    else
	    {
	        cout<<b<<endl;
	    }
	}
	return 0;
}

```