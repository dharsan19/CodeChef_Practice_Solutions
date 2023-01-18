# Fill the Bucket
## Problem
Chef has a bucket having a capacity of K liters. It is already filled with X liters of water.

Find the maximum amount of extra water in liters that Chef can fill in the bucket without overflowing.
## Input Format
The first line will contain T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains two space separated integers K and X - as mentioned in the problem.
## Output Format
For each test case, output in a single line, the amount of extra water in liters that Chef can fill in the bucket without overflowing.

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
	     cout<<x-y<<endl;
	 }
	return 0;
}
```