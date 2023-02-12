# Reach fast
## Problem
Chef is standing at coordinate A while Chefina is standing at coordinate B.

In one step, Chef can increase or decrease his coordinate by at most K.

Determine the minimum number of steps required by Chef to reach Chefina.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of three integers X,Y, and K, the initial coordinate of Chef, the initial coordinate of Chefina and the maximum number of coordinates Chef can move in one step.
## Output Format
For each test case, output the minimum number of steps required by Chef to reach Chefina.

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    long long int a,b,k;
	    cin>>a>>b>>k;
	    long long int step = abs(a-b);
        if(step%k == 0)
        {
            cout<<step/k<<endl;
        }
        else
        {
            cout<<(step/k)+1<<endl;
        }
	}
	return 0;
}
```