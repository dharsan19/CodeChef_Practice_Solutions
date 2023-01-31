# Blackjack
## Problem
Chef is playing a variant of Blackjack, where 3 numbers are drawn and each number lies between 1 and 10 (with both 1 and 10 inclusive). Chef wins the game when the sum of these 3 numbers is exactly 21.

Given the first two numbers A and B, that have been drawn by Chef, what should be 3-rd number that should be drawn by the Chef in order to win the game?

Note that it is possible that Chef cannot win the game, no matter what is the 3-rd number. In such cases, report −1 as the answer.

## Input Format
The first line will contain an integer T - number of test cases. Then the test cases follow.
The first and only line of each test case contains two integers A and B - the first and second number drawn by the Chef.
## Output Format
For each testcase, output the 3-rd number that should be drawn by the Chef in order to win the game. Output −1 if it is not possible for the Chef to win the game.

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
	    int total = a+b,count = 0;
	    for(int i =1; i<=10;i++)
	    {
	        if(total+i == 21)
	        {
	            cout<<i<<endl;
	            total = total+i;
	        }
	    }
	    if(total != 21)
	    {
	        cout<<-1<<endl;
	    }
	}
	return 0;
}
```