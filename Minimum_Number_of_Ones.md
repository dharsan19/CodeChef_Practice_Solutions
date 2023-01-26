# Minimum Number of Ones
## Problem
Your teacher gave you an assignment — given an integer N, construct a binary string B=b 1 b 2 b 3…b Nof length N such that: max(b i,b i+1)=1for every i from 1 to N−1.

What is the minimum number of 1's such a binary string can contain?

Note: A binary string is a string consisting of only the digits 0 and 1.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case contains a single integer N — the length of binary string you'd like to construct.
## Output Format
For each test case, output on a new line the minimum number of 1's required to complete the assignment.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int num;
	    cin>>num;
	    cout<<num/2<<endl;
	}
	return 0;
}
```