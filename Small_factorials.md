# Small factorials
## Problem
A tutorial for this problem is now available on our blog. Click here to read it.
You are asked to calculate factorials of some small positive integers.

## Input
An integer t, 1<=t<=100, denoting the number of testcases, followed by t lines, each containing a single integer n, 1<=n<=100.

## Output
For each integer n given at input, display a line with the value of n!

```cpp
#include <bits/stdc++.h>
#include <iostream>
#include <boost/multiprecision/cpp_int.hpp> 
using namespace boost::multiprecision; 
using namespace std;

int main() {
	// your code goes here
	int tc ;
	cin>>tc;
	while(tc--)
	{
	int n;
	cin>>n;
	cpp_int count = 1;
	for(int i = 1; i<=n; i++)
	{
	       count = count *i;
	       
	}
	cout <<count<<endl;
}
}
```