# Shopping Change
## Problem
Chef went shopping and bought items worth X rupees (1≤X≤100). Unfortunately, Chef only has a single 100 rupees note.

Since Chef is weak at maths, can you help Chef in calculating what money he should get back after paying 100 rupees for those items?

## Input Format
First line will contain T, the number of test cases. Then the test cases follow.
Each test case consists of a single line containing an integer X, the total price of items Chef purchased.
## Output Format
For each test case, output in a single line the money Chef has to receive back.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int rupees;
	    cin>>rupees;
	    cout<<100-rupees<<endl;
	}
	return 0;
}
```