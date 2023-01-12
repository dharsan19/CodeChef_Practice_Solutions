# Chef Plays Ludo
## Problem
Chef is playing Ludo. According to the rules of Ludo, a player can enter a new token into the play only when he rolls a 66 on the die.

In the current turn, Chef rolled the number XX on the die. Determine if Chef can enter a new token into the play in the current turn or not.

## Input Format
The first line contains a single integer TT — the number of test cases. Then the test cases follow.
The first and only line of each test case contains one integer XX — the number rolled by the Chef on the die.
## Output Format
For each test case, output YES if the Chef can enter a new token in the game. Otherwise, output NO.

You may print each character of YES and NO in uppercase or lowercase (for example, yes, yEs, Yes will be considered identical).
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x;
	    cin>>x;
	    if(x==6)
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
