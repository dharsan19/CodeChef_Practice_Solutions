# Test Score
## Problem
In a test, there are N problems, each carrying X marks.
In each problem, Chef either received X marks or 0 marks.

Determine whether is it possible for Chef to achieve exactly Y marks.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of three integers N,X, and Y, the number of problems, the maximum score for each problem, and the score Chef wants.
## Output Format
For each test case, output YES if Chef can achieve exactly Y marks, NO otherwise.

You can print each character of the string in uppercase or lowercase. For example, the strings Yes, YES, yes, and yEs, are all considered identical.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,x,y;
	    cin>>n;
	    cin>>x;
	    cin>>y;
        if((y>=x || y == 0) && y%x == 0)
        {
            cout<<"YES"<<endl;
        }
        else
        {
            cout<<"NO"<<endl;
        }
	}
	return 0;
}
```