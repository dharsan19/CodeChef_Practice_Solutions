# Expense List
## Problem
Chef has made a list for his monthly expenses. The list has N expenses with index 1 to N. The money spent on each expense depends upon the monthly income of Chef.

Chef spends 50% of his total income on the expense with index 1.
The money spent on the i thexpense (i>1) is equal to 50% of the amount remaining, after paying for all expenses with indices less than i.
Given that Chef earns 2 X rupees in a month, find the amount he saves after paying for all N expenses.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of two space-separated integers N and X — where N denotes the number of expenses and 2 X denotes the monthly income of Chef.
## Output Format
For each test case, output on a new line, the amount saved by Chef after paying for all N expenses.

```cpp
#include <iostream>
#include <math.h>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,salary,ans = 0;
	    cin>>a>>b;
	    salary = pow(2,b);
	    for(int i =0;i<a;i++)
	    {
	        ans = salary - salary/2;
	        salary = salary/2;
	    }
	    cout<<ans<<endl;
	}
	return 0;
}
```