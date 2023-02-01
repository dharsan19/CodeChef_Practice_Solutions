# It is My Serve
## Problem
Alice and Bob are playing a game of table tennis where irrespective of the point scored, every player makes 2 consecutive serves before the service changes. Alice makes the first serve of the match. Therefore the first 2 serves will be made by Alice, then the next 2 serves will be made by Bob and so on.

Let's consider the following example match for more clarity:

And the game continues 
…
…
After the score reaches P and Q for Alice and Bob respectively, both the players forgot whose serve it is. Help them determine whose service it is.

## Input Format
The first line contains a single integer T — the number of test cases. Then the test cases follow.
The first line of each test case contains two integers P and Q — the score of Alice and Bob respectively.
## Output Format
For each test case, determine which player's (Alice or Bob) serve it is.

You may print each character of Alice and Bob in uppercase or lowercase (for example, Bob, BOB, boB will be considered identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int p,q;
	    cin>>p>>q;
	    if((p+q)%2==0)
	    {
	        if(((p+q)/2)%2 == 0)
	        {
	            cout<<"Alice"<<endl;
	        }
	        else
	        {
	            cout<<"Bob"<<endl;
	        }
	    }
	    else
	    {
	        if((((p+q)/2)+1)%2 == 0)
	        {
	            cout<<"Bob"<<endl;
	        }
	        else
	        {
	            cout<<"Alice"<<endl;
	        }
	    }
	}
	return 0;
}
```