# Ranklist Pages
## Problem
Chef participated in a contest and got a rank X.

Chef is trying to find his name in the ranklist but there are too many pages.

Each page consists of 25 participants. Chef wants to find the exact page number which contains his name.
Help Chef find the page number.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of a single integer X - denoting the rank of Chef.
## Output Format
For each test case, output the page number of the ranklist containing Chef's name.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int rank;
	    cin>>rank;
	    if(rank%25 == 0)
	    {
	        cout<<rank/25<<endl;
	    }
	    else
	    {
	        cout<<(rank/25)+1<<endl;
	    }
	}
	return 0;
}
```