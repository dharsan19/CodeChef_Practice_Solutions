# Insurance
## Problem
Chef bought car insurance. The policy of the insurance is:

The maximum rebatable amount for any damage is Rs X lakhs.
If the amount required for repairing the damage is ≤X lakhs, that amount is rebated in full.
Chef's car meets an accident and required Rs Y lakhs for repairing.

Determine the amount that will be rebated by the insurance company.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
The first and only line of each test case contains two space-separated integers X and Y.
## Output Format
For each test case, output the amount (in lakhs) that will be rebated by the insurance company.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int insurance,accident;
	    cin>>insurance>>accident;
	    if(insurance > accident)
	    {
	        cout<<accident<<endl;
	    }
	    else
	    {
	        cout<<insurance<<endl;
	    }
	}
	return 0;
}
```