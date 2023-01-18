# Football Cup
## Problem
It is the final day of La Liga. Chef has a certain criteria for assessing football matches.
In particular, he only likes a match if:
The match ends in a draw, and,
At least one goal has been scored by either team.
Given the goals scored by both the teams as X and Y respectively, determine whether Chef will like the match or not.
## Input Format
The first line of input will contain a single integer T, denoting the number of test cases. The description of T test cases follows.
Each test case consists of a single line of input containing two space-separated integers X and Y — the goals scored by each team.
## Output Format
For each test case, output YES if Chef will like the match, else output NO.
You may print each character of the string in uppercase or lowercase (for example, the strings YeS, yEs, yes and YES will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y;
	    cin>>x>>y;
	    if(x==y && x>=1 && y>=1)
	    {
	        cout<<"YES"<<endl;
	    }
	    else
	    {
	        cout<<"NO"<<endl;
	    }
	}
	return 0;
}
```