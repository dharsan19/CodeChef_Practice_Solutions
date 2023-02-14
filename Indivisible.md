# Indivisible
## Problem
Alice thinks Bob has very weak math skills.
Alice gave Bob three numbers A,B, and C and challenged him to find any positive integer K strictly less than 100 such that none of the three numbers are divisible by K.

Help Bob find one such integer K.

Under the given constraints, a valid K will always exist.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
The first and only line of each test case contains three space-separated integers A,B, and C.
## Output Format
For each test case, output on a new line any positive integer K less than 100 that does not divide any of A,B, or C.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,c;
	    cin>>a>>b>>c;
	    for(int i=1;i<100;i++)
	    {
	        if(a%i!=0 && b%i!=0 && c%i!=0)
	        {
	            cout<<i<<endl;
	            break;
	        }
	    }
	}
	return 0;
}
```