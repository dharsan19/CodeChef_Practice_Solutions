# Minimum Cars required
## Problem
A single car can accommodate at most 4 people.

N friends want to go to a restaurant for a party. Find the minimum number of cars required to accommodate all the friends.

## Input Format
The first line contains a single integer T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains an integer N - denoting the number of friends.
## Output Format
For each test case, output the minimum number of cars required to accommodate all the friends.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int friends;
	    cin>>friends;
	    if(friends%4 == 0)
	    {
	        cout<<friends/4<<endl;
	    }
	    else
	    {
	        cout<<(friends/4)+1<<endl;
	    }
	}
	return 0;
}
```