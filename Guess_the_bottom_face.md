# Guess the bottom face
## Problem
It is known that in regular dice, the sum of opposite faces is 77.

A regular dice is rolled and you are given the value XX showing on the top face. Determine the value on the bottom face.

## Input Format
The first line will contain TT - the number of test cases. Then the test cases follow.
The first and only of each test case contains a single integer XX - the value on the top face.
## Output Format
For each test case, output the value on the bottom face.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x;
	    cin>>x;
	    cout<<7-x<<endl;
	}
	return 0;
}

```