# Volume Control
## Problem
Chef is watching TV. The current volume of the TV is X. Pressing the volume up button of the TV remote increases the volume by 1 while pressing the volume down button decreases the volume by 1. Chef wants to change the volume from X to Y. Find the minimum number of button presses required to do so.

## Input Format
The first line contains a single integer T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains two integers X and Y - the initial volume and final volume of the TV.
## Output Format
For each test case, output the minimum number of times Chef has to press a button to change the volume from X to Y.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y;
	    cin>>x>>y;
	    cout<<abs(x-y)<<endl;
	}
	return 0;
}
```