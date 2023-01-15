# Multivitamin Tablets
## Problem
The doctor prescribed Chef to take a multivitamin tablet 33 times a day for the next XX days.

Chef already has YY multivitamin tablets.

Determine if Chef has enough tablets for these XX days or not.

## Input Format
The first line contains a single integer TT — the number of test cases. Then the test cases follow.
The first and only line of each test case contains two space-separated integers XX and YY — the number of days Chef needs to take tablets and the number of tablets Chef already has.
## Output Format
For each test case, output YES if Chef has enough tablets for these XX days. Otherwise, output NO.

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
	    int x,y;
	    cin>>x>>y;
	    if(x*3 <= y)
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