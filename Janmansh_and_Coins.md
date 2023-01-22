# Janmansh and Coins
## Problem
Janmansh received X coins of 10 rupees and Y coins of 5 rupees from Chingari. Since he is weak in math, can you find out how much total money does he have?

## Input Format
The first line will contain T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains two integers X, Y - the number of 10 and 5 rupee coins respectively.
## Output Format
For each test case, output how much total money does Janmansh have.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y;
	    cin>>x>>y;
	    cout<<x*10 + y*5<<endl;
	}
	return 0;
}
```