# Sleep deprivation
## Problem
A person is said to be sleep deprived if he slept strictly less than 77 hours in a day.

Chef was only able to sleep XX hours yesterday. Determine if he is sleep deprived or not.

## Input Format
The first line contains a single integer TT — the number of test cases. Then the test cases follow.
The first and only line of each test case contains one integer XX — the number of hours Chef slept.
## Output Format
For each test case, output YES if Chef is sleep-deprived. Otherwise, output NO.

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
	    int sleep;
	    cin>>sleep;
	    if(sleep<7)
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