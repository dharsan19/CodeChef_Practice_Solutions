# Mana Points
## Problem
Chef is playing a mobile game. In the game, Chef's character Chefario can perform special attacks. However, one special attack costs X mana points to Chefario.

If Chefario currently has Y mana points, determine the maximum number of special attacks he can perform.

## Input Format
The first line contains a single integer T — the number of test cases. Then the test cases follow.
The first and only line of each test case contains two space-separated integers X and Y — the cost of one special attack and the number of mana points Chefario has initially.
## Output Format
For each test case, output the maximum number of special attacks Chefario can perform.

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
	    cout<<y/x<<endl;
	}
	return 0;
}
```