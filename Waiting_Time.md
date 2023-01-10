# Waiting Time
## Problem
Chef is eagerly waiting for a piece of information. His secret agent told him that this information would be revealed to him after KK weeks.

XX days have already passed and Chef is getting restless now. Find the number of remaining days Chef has to wait for, to get the information.

It is guaranteed that the information has not been revealed to the Chef yet.

## Input Format
The first line of input will contain an integer TT — the number of test cases. The description of TT test cases follows.
The first and only line of each test case contains two space-separated integers KK and XX, as described in the problem statement.
## Output Format
For each test case, output the number of remaining days that Chef will have to wait for.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int k,x,days;
	    cin>>k>>x;
	    days = (k*7) - x;
	    cout<<days<<endl;
	}
	return 0;
}
```