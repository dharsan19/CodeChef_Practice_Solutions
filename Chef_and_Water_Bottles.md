# Chef and Water Bottles
## Problem
Chef has N empty bottles where each bottle has a capacity of X litres.
There is a water tank in Chefland having K litres of water. Chef wants to fill the empty bottles using the water in the tank.

Assuming that Chef does not spill any water while filling the bottles, find out the maximum number of bottles Chef can fill completely.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains of a single line of input, three integers N,X, and K.
## Output Format
For each test case, output in a single line answer, the maximum number of bottles Chef can fill completely.

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
	    int ans = k/x;
	    if(ans <= n)
	    {
	        cout<<ans<<endl;
	    }
	    else
	    {
	        cout<<n<<endl;
	    }
	}
	return 0;
}
```