# Jenga Night
## Problem
Chef hosts a party for his birthday. There are N people at the party. All these N people decide to play Jenga.

There are X Jenga tiles available. In one round, all the players pick 1 tile each and place it in the tower.
The game is valid if:

All the players have a tile in each round;
All the tiles are used at the end.
Given N and X, find whether the game is valid.

## Input Format
First line will contain T, the number of test cases. Then the test cases follow.
Each test case contains a single line of input, containing two space-separated integers N and X representing the number of people at the party and the number of available tiles respectively.
## Output Format
For each test case, output in a single line YES if the game is valid, else output NO.

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
        int n,x;
        cin>>n>>x;
        if(n<=x && x%n == 0)
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