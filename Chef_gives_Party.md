# Chef gives Party
## Problem
Chef wants to give a burger party to all his NN friends i.e. he wants to buy one burger for each of his friends.

The cost of each burger is XX rupees while Chef has a total of KK rupees.

Determine whether he has enough money to buy a burger for each of his friends or not.

## Input Format
The first line contains a single integer TT - the number of test cases. Then the test cases follow.
The first and only line of each test case contains the three integers NN, XX, and KK - the number of Chef's friends, the cost of each burger, and the total money Chef has, respectively.
## Output Format
For each test case, output YES if the Chef can give a party to all his NN friends. Otherwise, output NO.

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
	    int n,x,k;
	    cin>>n>>x>>k;
	    if((n*x) <= k)
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