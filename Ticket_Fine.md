# Ticket Fine
## Problem
On a certain train, Chef-the ticket collector, collects a fine of Rs. XX if a passenger is travelling without a ticket. It is known that a passenger carries either a single ticket or no ticket.

PP passengers are travelling and they have a total of QQ tickets. Help Chef calculate the total fine collected.

## Input Format
The first line contains a single integer TT, the number of test cases. TT lines follow. Each following line contains three integers separated by spaces, whose description follows.

The first integer, XX, is the fee in rupees.
The second integer, PP, is the number of passengers on the train.
The third integer, QQ, is the number of tickets Chef collected.
## Output Format
The output must consist of TT lines.
The i^{th} line must contain a single integer, the total money(in rupees) collected by Chef corresponding to the i^{th}test case.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,p,q;
	    cin>>x>>p>>q;
	    cout<<x*(p-q)<<endl;
	}
	return 0;
}

```