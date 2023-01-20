# Bob at the Bank
## Problem
Bob has an account in the Bobby Bank. His current account balance is W rupees.

Each month, the office in which Bob works deposits a fixed amount of X rupees to his account.Y rupees is deducted from Bob's account each month as bank charges.

Find his final account balance after Z months. Note that the account balance can be negative as well.

## Input Format
The first line will contain T, the number of test cases. Then the test cases follow.
Each test case consists of a single line of input, containing four integers W,X,Y, and Z — the initial amount, the amount deposited per month, the amount deducted per month, and the number of months.
## Output Format
For each test case, output in a single line the final balance in Bob's account after Z months.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int w,x,y,z;
	    cin>>w>>x>>y>>z;
	    int balance;
	    balance = ((x-y)*z)+w;
	    cout<<balance<<endl;
	}
	return 0;
}
```