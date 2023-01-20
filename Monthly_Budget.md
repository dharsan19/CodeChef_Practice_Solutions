# Monthly Budget
## Problem
Akshat has X rupees to spend in the current month. His daily expenditure is Y rupees, i.e., he spends Y rupees each day.

Given that the current month has 30 days, find out if Akshat has enough money to meet his daily expenditures for this month.

## Input Format
The first line will contain T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains two integers X, Y - the amount of money Akshat has for the current month and his daily expenditure respectively.
## Output Format
For each test case, output YES if Akshat has enough money to meet his daily expenditure for 30 days of the month, otherwise output NO.

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
	    int x,y,ans;
	    cin>>x>>y;
	    ans = y*30;
	    if(x >= ans)
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