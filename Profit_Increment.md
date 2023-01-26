# Profit Increment
## Problem
Chef recently started selling a special fruit.
He has been selling the fruit for X rupees (X is a multiple of 100). He earns a profit of Y rupees on selling the fruit currently.

Chef decided to increase the selling price by 10%. Please help him calculate his new profit after the increase in selling price.

Note that only the selling price has been increased and the buying price is same.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of a single line of input containing two space-separated integers X and Y denoting the initial selling price and the profit respectively.
## Output Format
For each test case, output a single integer, denoting the new profit.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int selling_price, profit;
	    cin>>selling_price>>profit;
	    int new_price;
	    new_price = (selling_price) + ((selling_price)/10);
	    cout<<new_price - (selling_price - profit)<<endl;
	}
	return 0;
}
```