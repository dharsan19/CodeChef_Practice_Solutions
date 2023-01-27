# Determine the Winner
## Problem
There is a contest containing 2 problems A and B.
2 strong participants P and Q participated in the contest and solved both the problems.
P made AC submissions on problems A and B at time instants P A and P B respectively while Q made AC submissions on problems A and B at time instants Q Aand Q B.

It is given that the time penalty is the minimum time instant at which a participant has solved both the problems. Also the participant with the lower time penalty will have a better rank.

Determine which participant got the better rank or if there is a TIE.

## Input Format
The first line will contain T, number of test cases. Then the test cases follow.
Each test case contains a single line of input, four integers P A,P B,Q A,Q B.
## Output Format
For each test case, output P if P got a better rank, Q if Q got a better rank, TIE otherwise.

Note that output is case-insensitive i.e. P and p both are considered the same.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int p1,p2,q1,q2;
	    cin>>p1>>p2>>q1>>q2;
	    if(max(p1,p2) > max(q1,q2))
	    {
	        cout<<"Q"<<endl;
	    }
	    else if(max(p1,p2) < max(q1,q2))
	    {
	        cout<<"P"<<endl;
	    }
	    else
	    {
	        cout<<"TIE"<<endl;
	    }
	}
	return 0;
}
```