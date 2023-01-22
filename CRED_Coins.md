# CRED Coins
## Problem
For each bill you pay using CRED, you earn X CRED coins.
At CodeChef store, each bag is worth 100 CRED coins.

Chef pays Y number of bills using CRED. Find the maximum number of bags he can get from the CodeChef store.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains of a single line of input, two integers X and Y.
## Output Format
For each test case, output in a single line - the maximum number of bags Chef can get from the CodeChef store.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int cred,bills;
	    cin>>cred>>bills;
	    cout<<(cred*bills)/100<<endl;
	}
	return 0;
}

```