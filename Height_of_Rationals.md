# Height of Rationals
## Problem
In a recent breakthrough in mathematics, the proof utilized a concept called Height.

Consider a fraction a/b. Its Height is defined as the maximum of its numerator and denominator. So, for example, the Height of 3/19 would be 19, and the Height of 27/4 ​would be 27.

Given a and b, find the Height of a/b.

## Input Format
The only line of input contains two integers, a and b.
## Output Format
Output a single integer, which is the Height of a/b.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int numerator,denominator;
	cin>>numerator>>denominator;
	if(numerator>denominator)
	{
	    cout<<numerator;
	}
	else
	{
	    cout<<denominator;
	}
	return 0;
}
```