# Helping Chef
## Problem
Write a program, which takes an integer N and if the number is less than 10 then display "Thanks for helping Chef!" otherwise print "-1".

## Input Format
The first line contains an integer T, total number of testcases. Then follow T lines, each line contains an integer N.

## Output Format
For each test case, output the given string or -1 depending on conditions, in a new line.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n;
	    cin>>n;
	    if(n < 10)
	    {
	        cout<<"Thanks for helping Chef!"<<endl;
	    }
	    else
	    {
	        cout<<-1<<endl;
	    }
	}
	return 0;
}
```