# Best Coupon
## Problem
Chef is ordering food online (instead of cooking) and the bill comes out to be Rs. X. Chef can use one of the following two coupons to avail a discount.
Get 10 percent off on the bill amount
Get a flat discount of Rs. 100 on the bill amount
What is the maximum discount Chef can avail?

## Input Format
The first line contains a single integer T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains a single integer X - the bill amount before discount.
## Output Format
For each testcase, output the maximum discount Chef can avail.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x;
	    cin>>x;
	    if(x-100 < x-(x/100)*10)
	    {
	        cout<<100<<endl;
	    }
	    else
	    {
	        cout<<(x/100)*10<<endl;
	    }
	}
	return 0;
}
```