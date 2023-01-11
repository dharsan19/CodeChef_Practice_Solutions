# Equal Distribution
## Problem
Alice and Bob are very good friends and they always distribute all the eatables equally among themselves.

Alice has AA chocolates and Bob has BB chocolates. Determine whether Alice and Bob can distribute all the chocolates equally among themselves.

Note that:

It is not allowed to break a chocolate into more than one piece.
No chocolate shall be left in the distribution.
## Input Format
The first line of input will contain an integer TT — the number of test cases. The description of TT test cases follows.
The first and only line of each test case contains two space-separated integers AA and BB, the number of chocolates that Alice and Bob have, respectively.
## Output Format
For each test case, output on a new line \texttt{YES}YES if Alice and Bob can distribute all the chocolates equally, else output \texttt{NO}NO. The output is case insensitive, i.e, \texttt{yes}yes, \texttt{YeS}YeS, \texttt{yES}yES will all be accepted as correct answers when Alice and Bob can distribute the chocolates equally.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,total;
	    cin>>a>>b;
	    total = a+b;
	    if(total%2 == 0)
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