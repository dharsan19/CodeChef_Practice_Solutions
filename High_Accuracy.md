# High Accuracy
## Problem
There are 100 questions in a paper. Each question carries +3 marks for correct answer, -1 marks for incorrect answer and 0 marks for unattempted question.

It is given that Chef received exactly (0≤X≤100) marks. Determine the minimum number of problems Chef marked incorrect.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each testcase contains of a single integer X, marks that Chef received.
## Output Format
For each test case, output the minimum number of problems Chef marked incorrect.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int mark;
	    cin>>mark;
	    if(mark == 0)
	    {
	        cout<<0<<endl;
	    }
	    else if(mark%3 != 0)
	    {
	        cout<<3-(mark%3)<<endl;
	    }
	    else 
	    {
	        cout<<0<<endl;
	    }
	}
	return 0;
}
```