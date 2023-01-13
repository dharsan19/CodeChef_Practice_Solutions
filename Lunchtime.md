# Lunchtime
## Problem
Chef has his lunch only between 11 pm and 44 pm (both inclusive).

Given that the current time is XX pm, find out whether it is lunchtime for Chef.

## Input Format
The first line of input will contain a single integer TT, the number of test cases. Then the test cases follow.
Each test case contains a single line of input, containing one integer XX.
## Output Format
For each test case, print in a single line \texttt{YES}YES if it is lunchtime for Chef. Otherwise, print \texttt{NO}NO.

You may print each character of the string in either uppercase or lowercase (for example, the strings \texttt{YeS}YeS, \texttt{yEs}yEs, \texttt{yes}yes and \texttt{YES}YES will all be treated as identical).
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
	    if((x>=1) && (x<=4))
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