# Janmansh and Games
## Problem
Janmansh and Jay are playing a game. They start with a number X and they play a total of Y moves. Janmansh plays the first move of the game, after which both the players make moves alternatingly.

In one move, a player can increment or decrement X by 1.

If the final number after performing Y moves is even, then Janmansh wins otherwise, Jay wins. Determine the winner of the game if both the players play optimally.

## Input Format
The first line will contain T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains two integers X, Y - the starting number and the total number of moves respectively.
## Output Format
For each test case, output the winning player (Janmansh or Jay).

You may print each character of Janmansh and Jay in uppercase or lowercase (for example, JAY, jaY, JAy will be considered identical).

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
	    if(a%2==0 && b%2==0)
	    {
	        cout<<"Janmansh"<<endl;
	    }
	    else if(a%2!=0 && b%2!=0)
	    {
	        cout<<"Janmansh"<<endl;
	    }
	    else
	    {
	        cout<<"Jay"<<endl;
	    }
	}
	return 0;
}
```