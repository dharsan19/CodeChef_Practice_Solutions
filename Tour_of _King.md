# Tour of King
## Problem
King loves to go on tours with his friends.

King has NN cars that can seat 55 people each and MM cars that can seat 77 people each. Determine the maximum number of people that can travel together in these cars.

## Input Format
The first line of input contains a single integer TT, the number of test cases.
The first and only line of each test case contains two space-separated integers NN and MM — the number of 55-seaters and 77-seaters, respectively.
## Output Format
For each test case, output on a new line the maximum number of people that can travel together.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,m,tot;
	    cin>>n>>m;
	    tot = (n*5) + (m*7);
	    cout<<tot<<endl;
	}
	return 0;
}
```