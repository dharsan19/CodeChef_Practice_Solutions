# Zero String
## Problem
You are given a binary string S of length N. You are allowed to perform the following types of operations on string S:

Delete any one character from S, and concatenate the remaining parts of the string. For example, if we delete the third character of S=1101, it becomes S=111.
Flip all the characters of S. For example, if we flip all character of S=1101, it becomes S=0010.
Given that you can use either type of operation any number of times, find the minimum number of operations required to make all characters of the string S equal to 0.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of multiple lines of input.
The first line of each test case contains an integer N — the length of the string.
The next line contains a binary string S of length N.
## Output Format
For each test case, output on a new line, the minimum number of operations required to make all characters of the string S equal to 0.

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n;
	    cin>>n;
	    string str;
	    cin>>str;
	    int zero = 0,one = 0;
	    for(int i =0; i < n; i++)
	    {
	        if(str[i] == '0')
	            zero++;
	        else
	            one++;
	    }
	    cout<<min(one,zero+1)<<endl;
	    
	}
	return 0;
}
```