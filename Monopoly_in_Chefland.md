# Monopoly in Chefland
## Problem
Chef is the financial incharge of Chefland and one of his duties is identifying if any company has gained a monopolistic advantage in the market.

There are exactly 3 companies in the market each of whose revenues are denoted by R1,R2and R3 respectively. A company is said to have a monopolistic advantage if its revenue is strictly greater than the sum of the revenues of its competitors.

Given the revenue of the 3 companies, help Chef determine if any of them has a monopolistic advantage.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of a single line of input containing three space separated integers R1 R2 and R3denoting the revenue of the three companies respectively.
## Output Format
For each test case, output YES if any of the companies has a monopolistic advantage over its competitors, else output NO.

You may print each character of the string in uppercase or lowercase (for example, the strings YeS, yEs, yes and YES will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int r1,r2,r3;
	    cin>>r1>>r2>>r3;
	    if(r1 > r2+r3)
	    {
	        cout<<"Yes"<<endl;
	    }
	    else if(r2 > r1+r3)
	    {
	        cout<<"Yes"<<endl;
	    }
	    else if(r3 > r1+r2)
	    {
	        cout<<"Yes"<<endl;
	    }
	    else
	    {
	        cout<<"No"<<endl;
	    }
	}
	return 0;
}
```