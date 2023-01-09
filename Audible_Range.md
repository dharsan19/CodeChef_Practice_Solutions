# Audible Range
## Problem
Chef's dog binary hears frequencies starting from 6767 Hertz to 4500045000 Hertz (both inclusive).

If Chef's commands have a frequency of XX Hertz, find whether binary can hear them or not.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of a single integer XX - the frequency of Chef's commands in Hertz.
## Output Format
For each test case, output on a new line YES, if binary can hear Chef's commands. Otherwise, print NO.

The output is case-insensitive. Thus, the strings YES, yes, yeS, and Yes are all considered the same.
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
	    if(x>=67 and x<=45000)
	        cout<<"YES"<<endl;
	    else
	        cout<<"NO"<<endl;
	}
	return 0;
}
```