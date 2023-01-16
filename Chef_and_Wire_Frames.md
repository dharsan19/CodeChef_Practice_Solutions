# Chef and Wire Frames
## Problem
Chef has a rectangular plate of length Ncm and width Mcm. He wants to make a wireframe around the plate. The wireframe costs X rupees per cm.

Determine the cost Chef needs to incur to buy the wireframe.

## Input Format
First line will contain T, the number of test cases. Then the test cases follow.
Each test case consists of a single line of input, containing three space-separated integers N,M, and X — the length of the plate, width of the plate, and the cost of frame per cm.
## Output Format
For each test case, output in a single line, the price Chef needs to pay for the wireframe.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,m,x,total;
	    cin>>n>>m>>x;
	    total = (2*n + 2*m)*x;
	    cout<<total<<endl;
	    
	}
	return 0;
}

```