# Chairs Requirement
## Problem
Chef's coding class is very famous in Chefland.

This year XX students joined his class and each student will require one chair to sit on. Chef already has YY chairs in his class. Determine the minimum number of new chairs Chef must buy so that every student is able to get one chair to sit on.

## Input Format
The first line contains a single integer TT — the number of test cases. Then the test cases follow.
The first and only line of each test case contains two integers XX and YY — the number of students in the class and the number of chairs Chef already has.
## Output Format
For each test case, output the minimum number of extra chairs Chef must buy so that every student gets one chair.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--){
	    int x,y;
	    cin>>x>>y;
	    if(x>=y)
	        cout<<x-y<<endl;
	    else
	        cout<<0<<endl;
	}
	return 0;
}
```