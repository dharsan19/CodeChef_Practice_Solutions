# Chess Ratings
## Problem
Alice has recently started playing Chess. Her current rating is X. She noticed that when she wins a game, her rating increases by 8 points.

Can you help Alice in finding out the minimum number of games she needs to win in order to make her rating greater than or equal to Y?

## Input Format
The first line of input will contain an integer T — the number of test cases. The description of T test cases follows.
The first line of each test case contains two integers X and Y, as described in the problem statement.
## Output Format
For each test case, output the minimum number of games that Alice needs to win in order to make her rating greater than or equal to Y.

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
	    if((y-x)%8 == 0)
	    {
	        cout<<(y-x)/8<<endl;
	    }
	    else
	    {
	        cout<<((y-x)/8)+1<<endl;
	    }
	}
	return 0;
}
```