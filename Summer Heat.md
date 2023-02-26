# Summer Heat
## Problem
Read problem statements in Vietnamese,
Bengali, Mandarin Chinese, and Russian as well.

Chefland has 2 different types of coconut, type A and type B. Type A contains only x a  milliliters of coconut water and type B contains only x b grams of coconut pulp. Chef's nutritionist has advised him to consume X a  milliliters of coconut water and X b grams of coconut pulp every week in the summer. Find the total number of coconuts (type A + type B) that Chef should buy each week to keep himself active in the hot weather.

## Input Format
The first line contains an integer T, the number of test cases. Then the test cases follow.
Each test case contains a single line of input, four integers x a , x b , X a , X b .
## Output Format
For each test case, output in a single line the answer to the problem.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int xa,xb,ya,yb;
	    cin>>xa>>xb>>ya>>yb;
	    cout<<(ya/xa)+(yb/xb)<<endl;
	}
	return 0;
}
```