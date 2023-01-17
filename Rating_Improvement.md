# Rating Improvement
## Problem
Chef's current rating is X, and he wants to improve it. It is generally recommended that a person with rating X should solve problems whose difficulty lies in the range [X,X+200], i.e, problems whose difficulty is at least X and at most X+200.

You find out that Chef is currently solving problems with a difficulty of Y.

Is Chef following the recommended practice or not?

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases. The description of the test cases follows.
Each test case consists of a single line of input, containing two space-separated integers X,Y.
## Output Format
For each test case, output on a new line YES if Chef is following the recommended practice style, and NO otherwise.

Each letter of the output may be printed in either lowercase or uppercase. For example, the strings YES, yEs, and Yes will be considered identical.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int current_rating, difficulty;
	    cin>>current_rating>>difficulty;
	    if(difficulty >= current_rating && difficulty <= (current_rating+200))
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