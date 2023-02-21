# Good Quality Bulbs
## Problem
A bulb company claims that the average lifetime of its bulbs is at least X units.

The company ran a test on N bulbs. You are given the lifetime of N−1 of these bulbs. What is the minimum non-negative integer value of lifetime the remaining bulb can have, such that the claim of the company holds true?

## Input Format
The first line contains a single integer T - the number of test cases. Then the test cases follow.
The first line of each test case contains two integers N and X - denoting the number of test bulbs and the minimum average lifetime of bulbs in the company's claim.
The second line of each test case contains N−1 space-separated integers A 1 ,A 2 ,…,A N−1  denoting the lifetimes of N−1 of the test bulbs.
## Output Format
For each testcase, output the minimum non-negative integer value of lifetime the remaining bulb can have such that the claim of the company holds true.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,x,sum = 0;
	    cin>>n>>x;
	    for(int i =0;i<n-1;i++)
	    {
	        int a;
	        cin>>a;
	        sum +=a;
	    }
	    if((x*n) - sum >=0)
	    {
	        cout<<(x*n)-sum<<endl;
	    }
	    else
	    {
	        cout<<0<<endl;
	    }
	}
	return 0;
}
```