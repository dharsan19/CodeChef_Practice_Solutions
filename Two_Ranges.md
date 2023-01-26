# Two Ranges
## Problem
Chef has two ranges [A,B] and [C,D]. Chef needs to find the number of integers that belong to at least one of the ranges.

Note: A range [P,Q] contains all the integers {P,P+1,P+2,…,Q−1,Q}.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of a single line containing 4 integers A,B,C, and D, as mentioned in the statement.
## Output Format
For each test case, output on a new line, the number of integers that belong to at least one of the ranges.

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,c,d;
	    cin>>a>>b>>c>>d;
	    set<int>e;
	    for(int i=a; i<=b;i++)
	    {
	        e.insert(i);
	    }
	    for(int i=c; i<=d;i++)
	    {
	        e.insert(i);
	    }
	    cout<<e.size()<<endl;
	}
	return 0;
}
```