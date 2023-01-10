# Total Prize Money
## Problem
In a coding contest, there are prizes for the top rankers. The prize scheme is as follows:

Top 1010 participants receive rupees XX each.
Participants with rank 1111 to 100100 (both inclusive) receive rupees YY each.
Find the total prize money over all the contestants.

## Input Format
First line will contain TT, number of test cases. Then the test cases follow.
Each test case contains of a single line of input, two integers XX and YY - the prize for top 1010 rankers and the prize for ranks 1111 to 100100 respectively.
## Output Format
For each test case, output the total prize money over all the contestants.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y,total;
	    cin>>x>>y;
	    total = (x*10) + (y*90);
	    cout<<total<<endl;
	}
	return 0;
}
```