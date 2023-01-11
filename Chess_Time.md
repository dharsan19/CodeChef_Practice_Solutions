# Chess Time
## Problem
Chef has recently started playing chess, and wants to play as many games as possible.

He calculated that playing one game of chess takes at least 2020 minutes of his time.

Chef has NN hours of free time. What is the maximum number of complete chess games he can play in that time?

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of a single line containing a single integer, NN.
## Output Format
For each test case, output on a new line the maximum number of complete chess games Chef can play in NN hours.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,min;
	    cin>>n;
	    //converting hours into minutes
	    min = n*60;
	    cout<<min/20<<endl;
	}
	return 0;
}
```