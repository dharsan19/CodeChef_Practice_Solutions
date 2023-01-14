# Negative Product
## Problem
Chef is given three numbers A, B,A,B, and CC.

He wants to find whether he can select exactly two numbers out of these such that the product of the selected numbers is negative.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of three integers A, B,A,B, and CC, the given numbers.
## Output Format
For each test case, output YES if Chef can select exactly two numbers out of these such that the product of the selected numbers is negative, NO otherwise.

You may print each character in uppercase or lowercase. For example, the strings NO, no, No, and nO, are all considered identical.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,c;
	    cin>>a>>b>>c;
	    if(a>=0 && b>=0 && c>=0)
	    {
	        cout<<"NO"<<endl;
	    }
	    else if(a<=0 && b<=0 && c<=0)
	    {
	        cout<<"NO"<<endl;
	    }
	    else
	    {
	        cout<<"YES"<<endl;
	    }
	}
	return 0;
}
```