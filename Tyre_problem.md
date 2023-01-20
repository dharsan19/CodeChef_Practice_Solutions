# Tyre problem
## Problem
There are N bikes and M cars on the road.

Each bike has 2 tyres.
Each car has 4 tyres.
Find the total number of tyres on the road.

## Input Format
The first line will contain T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains two integers N,M.
## Output Format
For each test case, output in a single line, the total number of tyres on the road.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int bike,car,tyre;
	    cin>>bike>>car;
	    tyre = bike*2 + car*4;
	    cout<<tyre<<endl;
	}
	return 0;
}
```