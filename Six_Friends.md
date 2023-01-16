# Six Friends
## Problem
Six friends go on a trip and are looking for accommodation. After looking for hours, they find a hotel which offers two types of rooms — double rooms and triple rooms. A double room costs Rs. X, while a triple room costs Rs.Y.

The friends can either get three double rooms or get two triple rooms. Find the minimum amount they will have to pay to accommodate all six of them.

## Input Format
The first line contains a single integer T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains two integers X and Y - the cost of a double room and the cost of a triple room.
## Output Format
For each testcase, output the minimum amount required to accommodate all the six friends.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int dou,tri;
	    cin>>dou>>tri;
	    if(dou*3 < tri*2)
	    {
	        cout<<dou*3<<endl;
	    }
	    else
	    {
	        cout<<tri*2<<endl;
	    }
	}
	return 0;
}

```