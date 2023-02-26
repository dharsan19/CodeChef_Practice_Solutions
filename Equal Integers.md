# Equal Integers
## Problem
Chef has two integers X and Y. Chef wants to perform some operations to make X and Y equal. In one operation, Chef can either:
set X:=X+1 or set Y:=Y+2
Find the minimum number of operations required to make X and Y equal.

## Input Format
The first line contains a single integer T — the number of test cases. Then the test cases follow.
The first and only line of each test case contains two space separated integers X and Y.
## Output Format
For each test case, print the minimum number of operations required to make X and Y equal.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y,count = 0;
	    cin>>x>>y;
	    if(x>y)
	    {
	        while(x>y)
	        {
	            y = y+2;
	            count++;
	        }
	        if(x == y)
	        {
	            cout<<count<<endl;
	        }
	        else if(y > x)
	        {
	            cout<<count+(y-x)<<endl;
	        }
	        else
	        {
	            cout<<0<<endl;
	        }
	    }
	    else
	    {
	        while(y > x)
	        {
	            x = x+1;
	            count++;
	        }
	        if(x == y)
	        {
	            cout<<count<<endl;
	        }
	        else
	        {
	            cout<<0<<endl;
	        }
	    }
	}
	return 0;
}
```