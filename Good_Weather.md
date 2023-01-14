# Good Weather
## Problem
The weather report of Chefland is Good if the number of sunny days in a week is strictly greater than the number of rainy days.
## Input Format
First line will contain TT, number of testcases. Then the testcases follow.
Each testcase contains of a single line of input, 77 space separated integers
## Output Format
For each testcase, print "YES" if the weather report of Chefland is Good, otherwise print "NO". Print the output without quotes.

You may print each character of the string in uppercase or lowercase (for example, the strings "yEs", "yes", "Yes" and "YES" will all be treated as identical).
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int count = 0,a;
	    for(int i = 0;i<=6;i++)
	    {
	        cin>>a;
	        if(a==1)
	        {
	            count++;
	        }
	        else 
	        {
	            continue;
	        }
	    }
	    if(count>=4)
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