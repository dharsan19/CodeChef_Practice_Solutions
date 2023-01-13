# Chef and Chapters
## Problem
This semester, Chef took XX courses. Each course has YY units and each unit has ZZ chapters in it.

Find the total number of chapters Chef has to study this semester.

## Input Format
The first line will contain TT, the number of test cases. Then the test cases follow.
Each test case consists of a single line of input, containing three space-separated integers X, Y,X,Y, and ZZ.
## Output Format
For each test case, output in a single line the total number of chapters Chef has to study this semester.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y,z;
	    cin>>x>>y>>z;
	    cout<<x*y*z<<endl;
	}
	return 0;
}
```