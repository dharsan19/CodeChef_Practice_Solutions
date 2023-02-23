# Make A and B equal
## Problem
Chef has two numbers A and B.

In one operation, Chef can choose either A or B and multiply it by 2.

Determine whether he can make both A and B equal after any number (possibly, zero) of moves.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of two space-separated integers A and B.
## Output Format
For each test case, output YES if Chef can make both numbers equal, NO otherwise.

Note that the checker is case-insensitive i.e. YES, Yes, yes, yES are all considered same.

```cpp
#include <iostream>
#include<cmath>
using namespace std;

int main() 
{
	int i,t,a,b,j;
	cin>>t;
	for(i=1;i<=t;i++)
	{
	    cin>>a>>b;
	    if(a==b)
	    cout<<"yes"<<endl;
	    else if(a<b)
	    {
	        for(j=1;;j++)
	        {
	            a=a*2;
	            if(a==b)
	            {
	                cout<<"yes"<<endl;
	                break;
	            }
	            else if(a>b)
	            {
	              cout<<"no"<<endl;
	              break;
	            }
	        }
	    }
	    else
	    {
	       for(j=1;;j++)
	        {
	            b=b*2;
	            if(a==b)
	            {
	                cout<<"yes"<<endl;
	                break;
	            }
	            else if(b>a)
	            {
	              cout<<"no"<<endl;
	              break;
	            }
	        } 
	    }
	    
	}
	return 0;
}
```