# Maximum Submissions
## Problem
A participant can make 1 submission every 30 seconds. If a contest lasts for X minutes, what is the maximum number of submissions that the participant can make during it?

It is also given that the participant cannot make any submission in the last 5 seconds of the contest.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of a single integer X, denoting the number of minutes.
## Output Format
For each test case, output the maximum number of submissions a participant can make in X minutes.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int minutes;
	    cin>>minutes;
	    cout<<minutes*2<<endl;
	}
	return 0;
}
```