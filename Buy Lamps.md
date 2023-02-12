# Buy Lamps
## Problem
An electronics shop sells red and blue lamps. A red lamp costs X rupees and a blue lamp costs Y rupees.

Chef is going to buy exactly N lamps from this shop. Find the minimum amount of money Chef needs to pay such that at least K of the lamps bought are red.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of a single line containing four space-separated integers N,K,X,Y.
## Output Format
For each test case, output on a new line the minimum amount of money Chef needs to pay in order to buy N lamps such that at least K of the lamps bought are red.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,k,x,y;
	    cin>>n;
	    cin>>k;
	    cin>>x;
	    cin>>y;
	    int min = (k*x);
	    int ans1 = (n-k)*x;
	    int ans2 = (n-k)*y;
	    if(ans1 <= ans2)
	    {
	        cout<<ans1+min<<endl;
	    }
	    else
	    {
	        cout<<ans2+min<<endl;
	    }
	}
	return 0;
}
```