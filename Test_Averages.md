# Test Averages
## Problem
Chef has scored A,B, and C marks in 3 different subjects respectively.

Chef will fail if the average score of any two subjects is less than 35. Determine whether Chef will pass or fail.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains of a single line of input, three integers A,B,C, denoting the Chef's score in the three subjects.
## Output Format
For each test case, if Chef will pass, print PASS, otherwise print FAIL.

You may print each character of the string in uppercase or lowercase (for example, the strings pass, Pass, pAss, and PASS will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,c;
	    cin>>a>>b>>c;
	    if(a+b >= 70 && b+c >=70 && c+a >=70)
	    {
	        cout<<"Pass"<<endl;
	    }
	    else
	    {
	        cout<<"Fail"<<endl;
	    }
	}
	return 0;
}
```