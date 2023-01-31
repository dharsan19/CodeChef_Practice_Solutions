# Change Row and Column Both
## Problem
There is a 10×10 grid with rows numbered 1 to 10 from top to bottom, and columns 1 to 10 from left to right. Each cell is identified by a pair (r, c) which means that the cell is located at row r and column c.

If Chef's current location is (a,b), then in one move Chef can go to (c,d) if both of the following are satisfied:
a≠c
b≠d
Determine the minimum number of moves required to go from (s x,s y) to (e x,e y).

## Input Format
The first line contains a single integer 
T — the number of test cases. Then the test cases follow.
The first and only line of each test case contains four integer s x, s y, e x, e y— the coordinates of the starting and ending cells.
## Output Format
For each testcase, output the minimum number of moves required to go from (s x,s y) to (e x,e y).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,c,d;
	    cin>>a>>b>>c>>d;
	    if(a == c || b == d)
	    {
	        cout<<2<<endl;
	    }
	    else
	    {
	        cout<<1<<endl;
	    }
	}
	return 0;
}
```