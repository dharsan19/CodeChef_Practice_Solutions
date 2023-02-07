# A or B
## Problem
There are two problems in a contest.

Problem A is worth 500 points at the start of the contest.
Problem B is worth 1000 points at the start of the contest.
Once the contest starts, after each minute:

Maximum points of Problem A reduce by 2 points .
Maximum points of Problem B reduce by 4 points.
It is known that Chef requires X minutes to solve Problem A correctly and Y minutes to solve Problem B correctly.

Find the maximum number of points Chef can score if he optimally decides the order of attempting both the problems.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains of a single line of input, two integers X and Y - the time required to solve problems A and B in minutes respectively.
## Output Format
For each test case, output in a single line, the maximum number of points Chef can score if he optimally decides the order of attempting both the problems.

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
	    int ans1 = (500-(a*2)) + (1000-((a+b)*4));
	    int ans2 = (500-(a+b)*2) + (1000-(b*4));
	    cout<<max(ans1,ans2)<<endl;
	}
	return 0;
}
```