# Chessboard Distance
## Problem
The Chessboard Distance for any two points (X 1,Y 1) and (X 2,Y 2) on a Cartesian plane is defined as max(∣X 1−X 2∣,∣Y 1−Y 2∣).

You are given two points (X 1,Y 1) and (X 2,Y 2). Output their Chessboard Distance.

Note that, ∣P∣ denotes the absolute value of integer P. 

## Input Format
First line will contain T, the number of test cases. Then the test cases follow.
Each test case consists of a single line of input containing 4 space separated integers - X 1,Y 1,X 2,Y 2- as defined in the problem statement.
## Output Format
For each test case, output in a single line the chessboard distance between (X 1,Y 1) and (X 2,Y 2)

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int T;
	cin>>T;
	while(T--)
	{
	    int X1,Y1,X2,Y2,ans;
	    cin>>X1>>Y1>>X2>>Y2;
        ans = max(abs(X1-X2),abs(Y1-Y2));
        cout<<ans<<endl;
	}
	return 0;
}

```