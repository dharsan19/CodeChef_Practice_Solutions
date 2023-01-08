# Kitchen Timings
# Problem
The working hours of Chef’s kitchen are from XX pm to YY pm (1 \le X \lt Y \le 12)(1≤X<Y≤12).

Find the number of hours Chef works.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of two space-separated integers XX and YY — the starting and ending time of working hours respectively.
## Output Format
For each test case, output on a new line, the number of hours Chef works.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y,hours;
	    cin>>x>>y;
	    hours = y-x;
	    cout<<hours<<endl;
	}
	return 0;
}
```