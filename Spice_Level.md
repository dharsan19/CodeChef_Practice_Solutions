# Spice Level
## Problem
Each item in Chef’s menu is assigned a spice level from 1 to 10. Based on the spice level, the item is categorised as:

MILD: If the spice level is less than 4.
MEDIUM: If the spice level is greater than equal to 4 but less than 7.
HOT: If the spice level is greater than equal to 7.
Given that the spice level of an item is X, find the category it lies in.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of an integer X — the spice level of the item.
## Output Format
For each test case, output on a new line, the category that the item lies in.

You may print each character in uppercase or lowercase. For example, HOT, hot, Hot, and hOT are all considered the same.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int spice;
	    cin>>spice;
	    if(spice < 4)
	    {
	        cout<<"MILD"<<endl;
	    }
	    else if(spice >= 4 && spice < 7)
	    {
	        cout<<"MEDIUM"<<endl;
	    }
	    else
	    {
	        cout<<"HOT"<<endl;
	    }
	}
	return 0;
}

```