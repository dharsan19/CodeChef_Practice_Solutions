# Read Pages
## Problem
Chef has started studying for the upcoming test. The textbook has N pages in total. Chef wants to read at most X pages a day for Y days.

Find out whether it is possible for Chef to complete the whole book.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
The first and only line of each test case contains three space-separated integers N,X, and Y — the number of pages, the number of pages Chef can read in a day, and the number of days.
## Output Format
For each test case, output on a new line, YES, if Chef can complete the whole book in given time, and NO otherwise.

You may print each character of the string in uppercase or lowercase. For example, Yes, YES, yes, and yES are all considered identical.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,x,y;
	    cin>>n>>x>>y;
	    if(n <= x*y)
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