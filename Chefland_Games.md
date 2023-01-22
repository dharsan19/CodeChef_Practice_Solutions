# Chefland Games
## Problem
In Chefland, a tennis game involves 4 referees.
Each referee has to point out whether he considers the ball to be inside limits or outside limits. The ball is considered to be IN if and only if all the referees agree that it was inside limits.

Given the decision of the 4 referees, help Chef determine whether the ball is considered inside limits or not.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of a single line of input containing 4 integers R 1,R 2,R 3,R 4 denoting the decision of the respective referees.
Here R can be either 0 or 1 where 0 would denote that the referee considered the ball to be inside limits whereas 1 denotes that they consider it to be outside limits.

## Output Format
For each test case, output IN if the ball is considered to be inside limits by all referees and OUT otherwise.

The checker is case-insensitive so answers like in, In, and IN would be considered the same.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int ball,count = 0;
	    for(int i =0; i<4; i++)
	    {
	        cin>>ball;
	        if(ball == 0)
	        {
	            count++;
	        }
	    }
	    if(count == 4)
	    {
	        cout<<"IN"<<endl;
	    }
	    else
	    {
	        cout<<"OUT"<<endl;
	    }
	}
	return 0;
}
```