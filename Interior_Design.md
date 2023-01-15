# Interior Design
## Problem
Chef decided to redecorate his house, and now needs to decide between two different styles of interior design.
For the first style, tiling the floor will cost X_1 rupees and painting the walls will cost Y_1 rupees.
For the second style, tiling the floor will cost X_2 rupees and painting the walls will cost Y_2 rupees.
Chef will choose whichever style has the lower total cost. How much will Chef pay for his interior design?

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of a single line of input, containing 44 space-separated integers X_1, Y_1, X_2, Y_2 as described in the statement.
## Output Format
For each test case, output on a new line the amount Chef will pay for interior design.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x1,y1,x2,y2;
	    cin>>x1>>y1>>x2>>y2;
	    if(x1+y1 < x2+y2)
	    {
	        cout<<x1+y1<<endl;
	    }
	    else
	    {
	        cout<<x2+y2<<endl;
	    }
	}
	return 0;
}
```