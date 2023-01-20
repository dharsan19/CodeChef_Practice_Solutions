# Practice makes us perfect
## Problem
Most programmers will tell you that one of the ways to improve your performance in competitive programming is to practice a lot of problems.

Our Chef took the above advice very seriously and decided to set a target for himself.

Chef decides to solve at least 10 problems every week for 4 weeks.
Given the number of problems he actually solved in each week over 4 weeks as P1,P2,P3, and P4, output the number of weeks in which Chef met his target.

## Input Format
There is a single line of input, with 4 integers P1,P2,P3, and P 4. These are the number of problems solved by Chef in each of the 4 weeks.

## Output Format
Output a single integer in a single line - the number of weeks in which Chef solved at least 10 problems.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int arr[4],count = 0;
	for(int i=0;i<4;i++)
	{
	    cin>>arr[i];
	    if(arr[i] >= 10)
	    {
	        count++;
	    }
	}
	cout<<count;
	return 0;
}
```