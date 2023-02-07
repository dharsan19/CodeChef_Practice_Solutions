# Count the ACs
## Problem
There are 10 problems in a contest. You know that the score of each problem is either 1 or 100 points.

Chef came to know the total score of a participant and he is wondering how many problems were actually solved by that participant.

Given the total score P of the participant, determine the number of problems solved by the participant. Print −1 in case the score is invalid.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains of a single line containing a single integer P - denoting the number of points scored by the participant.
## Output Format
For each testcase, output the number of problems solved by the participant or −1 if the score is invalid.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x;
	    cin>>x;
	    if(x%100 > 10-(x/100))
	    {
	        cout<<-1<<endl;
	    }
	    else
	    {
	        cout<<(x/100)+(x%100)<<endl;
	    }
	}
	return 0;
}
```