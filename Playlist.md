# Playlist
## Problem
Chef's playlist contains 3 songs named A,B, and C, each of duration exactly X minutes. Chef generally plays these 3 songs in loop, i.e, A→B→C→A→B→C→A→…

Chef went on a train journey of N minutes and played his playlist on loop for the whole journey. How many times did he listen to the song C completely?

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases. The description of the test cases follows.
Each test case consists of a single line of input, containing two space-separated integers N,X.
## Output Format
For each test case, output on a new line the number of times Chef listens to the song C completely.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,x;
	    cin>>n>>x;
	    cout<<n/(x*3)<<endl;
	}
	return 0;
}
```