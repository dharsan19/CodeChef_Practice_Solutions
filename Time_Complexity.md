# Time Complexity
## Problem
A sorting algorithm AA is said to have more time complexity than a sorting algorithm BB if it uses more number of comparisons for sorting the same array than algorithm BB.

Given that algorithm AA uses XX comparisons to sort an array and algorithm BB uses YY comparisons to sort the same array, find whether algorithm AA has more time complexity.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of two space-separated integers XX and YY — the number of comparisons used by algorithms AA and BB to sort the array respectively.
## Output Format
For each test case, output on a new line, YES, if the algorithm AA has more time complexity than BB and NO otherwise.

You may print each character of the string in uppercase or lowercase (for example, the strings YES, yEs, yes, and yeS will all be treated as identical).
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b;
	    cin>>a>>b;
	    if(a>b)
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