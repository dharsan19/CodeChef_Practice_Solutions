# The Mango Truck
## Problem
You are given that a mango weighs X kilograms and a truck weighs Y kilograms. You want to cross a bridge that can withstand a weight of Z kilograms.

Find the maximum number of mangoes you can load in the truck so that you can cross the bridge safely.

## Input Format
First line will contain T, the number of test cases. Then the test cases follow.
Each test case consists of a single line of input, three integers X,Y,Z - the weight of mango, the weight of truck and the weight the bridge can withstand respectively.
## Output Format
For each test case, output in a single line the maximum number of mangoes that you can load in the truck.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y,z;
	    cin>>x>>y>>z;
	    int ans;
	    ans = (z-y)/x;
	    cout<<ans<<endl;
	}
	return 0;
}
```