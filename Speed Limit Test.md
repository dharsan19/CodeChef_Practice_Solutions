# Speed Limit Test
## Problem
Alice is driving from her home to her office which is A kilometers away and will take her X hours to reach.
Bob is driving from his home to his office which is B kilometers away and will take him Y hours to reach.

Determine who is driving faster, else, if they are both driving at the same speed print EQUAL.

## Input Format
The first line will contain T, the number of test cases. Then the test cases follow.
Each test case consists of a single line of input, containing four integers A,X,B, and Y, the distances and and the times taken by Alice and Bob respectively.
## Output Format
For each test case, if Alice is faster, print ALICE. Else if Bob is faster, print BOB. If both are equal, print EQUAL.

You may print each character of the string in uppercase or lowercase (for example, the strings equal, equAL, EquAl, and EQUAL will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    float a,x,b,y;
	    cin>>a>>x>>b>>y;
	    if((a/x)>(b/y))
	    {
	        cout<<"Alice"<<endl;
	    }
	    else if((a/x)<(b/y))
	    {
	        cout<<"Bob"<<endl;
	    }
	    else
	    {
	        cout<<"Equal"<<endl;
	    }
	}
	return 0;
}
```