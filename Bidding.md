# Bidding
## Problem
Alice, Bob and Charlie are bidding for an artifact at an auction.
Alice bids AA rupees, Bob bids BB rupees, and Charlie bids CC rupees (where AA, BB, and CC are distinct).

According to the rules of the auction, the person who bids the highest amount will win the auction.
Determine who will win the auction.

## Input Format
The first line contains a single integer TT — the number of test cases. Then the test cases follow.
The first and only line of each test case contains three integers AA, BB, and CC, — the amount bid by Alice, Bob, and Charlie respectively.
## Output Format
For each test case, output who (out of Alice, Bob, and Charlie) will win the auction.

You may print each character of Alice, Bob, and Charlie in uppercase or lowercase (for example, ALICE, aliCe, aLIcE will be considered identical).
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
	    if((a>b) && (a>c))
	    {
	        cout<<"Alice"<<endl;
	    }
	    else if((b>a) && (b>c))
	    {
	        cout<<"Bob"<<endl;
	    }
	    else
	    {
	        cout<<"Charlie"<<endl;
	    }
	}
	return 0;
}
```