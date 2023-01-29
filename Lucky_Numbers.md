# Lucky Numbers
## Problem
Chef calls a number lucky if it contains the digit 7 at least once.

Given a number X, determine if it is a lucky number or not.

## Input Format
The first line contains a single integer T — the number of test cases. Then the test cases follow.
The first and only line of each test case contains an integer X — the number mentioned in the problem statement.
## Output Format
For each test case, output YES if X is a lucky number. Otherwise, output NO.

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
	    int num,count = 0;
	    cin>>num;
	    while(num > 0)
	    {
	        if(num%10 == 7)
	        {
	            count++;
	        }
	        num = num/10;
	    }
	    if(count>=1)
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