# Integers that sum to the same value
## Problem
Alice has a positive integer N. She is wondering how many ordered pairs of positive integers (i,j) exist such that i+j=N.

Help Alice figure out the answer.

Note that since the pairs are ordered, (1,2) and (2,1) are considered different.

## Input Format
The first and only line of input contains a single integer N.

## Output Format
Print a single integer, the number of ordered pairs of positive integers (i,j) such that i+j=N.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int num;
	cin>>num;
	int count = 0;
	for(int i =1; i<num; i++)
	{
	    for(int j =1; j<num; j++)
	    {
	        if(i+j == num)
	        {
	            count++;
	        }
	    }
	}
	cout<<count<<endl;
	return 0;
}
```