# Bull or Bear
## Problem
Chef is on his way to become the new big bull of the stock market but is a bit weak at calculating whether he made a profit or a loss on his deal.

Given that Chef bought the stock at value XX and sold it at value YY. Help him calculate whether he made a profit, loss, or was it a neutral deal.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of a single line of input containing two space-separated integers XX and YY, denoting the value at which Chef bought and sold the stock respectively.
## Output Format
For each test case, output PROFIT if Chef made a profit on the deal, LOSS if Chef incurred a loss on the deal, and NEUTRAL otherwise.

The checker is case-insensitive so answers like pROfiT, profit, and PROFIT would be considered the same. 
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
	    if(x>y)
	        cout<<"LOSS"<<endl;
	    else if (y>x)
	        cout<<"PROFIT"<<endl;
	    else
	        cout<<"NEUTRAL"<<endl;
	}
	return 0;
}
```