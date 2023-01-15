# Far from origin
## Problem
Alice, Bob, and, Chef are standing on the coordinate plane. Chef is standing at the origin (coordinates (0, 0)(0,0)) while the location of Alice and Bob are (X_1, Y_1) and (X_2, Y_2) respectively.

Amongst Alice and Bob, find out who is at a farther distance from Chef or determine if both are at the same distance from Chef.
## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
The first and only line of each test case contains four space-separated integers X_1, Y_1, X_2,the coordinates of Alex and Bob.
## Output Format
For each test case, output on a new line:

ALEX, if Alex is at a farther distance from Chef.
BOB, if Bob is at a farther distance from Chef.
EQUAL, if both are standing at the same distance from Chef.
You may print each character in uppercase or lowercase. For example, Bob, BOB, bob, and bOB, are all considered identical.
```cpp
#include <iostream>
#include <math.h>
#include <cmath>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    float a1,a2,b1,b2,alex,bob;
	    cin>>a1>>a2>>b1>>b2;
	    alex = sqrt(pow(a1,2) + pow(a2,2));
	    bob = sqrt(pow(b1,2) + pow(b2,2));
	    if(alex>bob)
	    {
	        cout<<"ALEX"<<endl;
	    }
	    else if(bob>alex)
	    {
	        cout<<"BOB"<<endl;
	    }
	    else
	    {
	        cout<<"EQUAL"<<endl;
	    }
	    
	}
	return 0;
}
```