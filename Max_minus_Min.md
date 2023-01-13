# Max minus Min
## Problem
Chef is given 33 integers A, B,A,B, and CC such that A \lt B \lt CA<B<C.

Chef needs to find the value of max(A, B, C) - min(A, B, C)max(A,B,C)−min(A,B,C).

Here max(A, B, C)max(A,B,C) denotes the maximum value among A, B, CA,B,C while min(A, B, C)min(A,B,C) denotes the minimum value among A, B, CA,B,C.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of 33 integers A, B, CA,B,C.
## Output Format
For each test case, output the value of max(A, B, C) - min(A, B, C)max(A,B,C)−min(A,B,C).
```cpp
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,c,maxi,mini;
	    cin>>a>>b>>c;
	    maxi = max(c,max(a,b));
	    mini = min(c,min(a,b));
	    cout<<maxi-mini<<endl;
	}
	return 0;
}
```