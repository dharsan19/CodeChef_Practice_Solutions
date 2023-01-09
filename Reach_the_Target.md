# Reach the Target
## Problem
There is a cricket match going on between two teams AA and BB.

Team BB is batting second and got a target of XX runs. Currently, team BB has scored YY runs. Determine how many more runs Team BB should score to win the match.

Note: The target score in cricket matches is one more than the number of runs scored by the team that batted first.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of two space-separated integers XX and YY, the target for team BB and the current score of team BB respectively.
## Output Format
For each test case, output how many more runs team BB should score to win the match.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y,to_win;
	    cin>>x>>y;
	    to_win = x-y;
	    cout<<to_win<<endl;
	}
	return 0;
}

```