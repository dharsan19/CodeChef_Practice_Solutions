# DNA Storage
## Problem
For encoding an even-length binary string into a sequence of A, T, C, and G, we iterate from left to right and replace the characters as follows:

00 is replaced with A
01 is replaced with T
10 is replaced with C
11 is replaced with G
Given a binary string S of length N (N is even), find the encoded sequence.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains two lines of input.
First line contains a single integer N, the length of the sequence.
Second line contains binary string S of length N.
## Output Format
For each test case, output in a single line the encoded sequence.

Note: Output is case-sensitive.

```cpp
#include <iostream>
#include <string.h>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n;
	    cin>>n;
	    string s;
	    cin>>s;
	    for(int i =0; i<n;i+=2)
	    {
	        if(s[i] == '0' && s[i+1] == '0') 
	            cout<<"A";
	        else if(s[i] == '0' && s[i+1] == '1')
	            cout<<"T";
	        else if(s[i] == '1' && s[i+1] == '0')
	            cout<<"C";
	        else
	            cout<<"G";
	    }
	    cout<<endl;
	    
	}
	return 0;
}
```