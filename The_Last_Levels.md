# The Last Levels
## Problem
Chef is playing a videogame, and is getting close to the end. He decides to finish the rest of the game in a single session.

There are X levels remaining in the game, and each level takes Chef Y minutes to complete. To protect against eye strain, Chef also decides that every time he completes 3 levels, he will take a Z minute break from playing. Note that there is no need to take this break if the game has been completed.

How much time (in minutes) will it take Chef to complete the game?

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
The first and only line of input will contain three space-separated integers X, Y, and Z.
## Output Format
For each test case, output on a new line the answer — the length of Chef's gaming session.

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
	    int ans = (a*b) + ((a/3)*c);
	    if(a%3 == 0)
	    {
	        cout<<ans-c<<endl;
	    }
	    else
	    {
	        cout<<ans<<endl;
	    }
	}
	return 0;
}
```