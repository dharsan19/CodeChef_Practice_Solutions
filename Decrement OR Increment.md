# Decrement OR Increment
## Problem
Write a program to obtain a number N and increment its value by 1 if the number is divisible by 4 otherwise decrement its value by 1.

## Input Format
First line will contain a number N.

## Output Format
Output a single line, the new value of the number.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int n;
	cin>>n;
	if(n%4 == 0)
	{
	    cout<<n+1<<endl;
	}
	else
	{
	    cout<<n-1<<endl;
	}
	return 0;
}
```