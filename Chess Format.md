# Chess Format
## Problem
Read problem statements in Russian and Mandarin Chinese.
Given the time control of a chess match as a+b, determine which format of chess out of the given 4 it belongs to.

1) Bullet if a+b<3
2) Blitz if ≤a+b≤10
3) Rapid if 11≤a+b≤60
4) Classical if 60 < a+b

## Input Format
First line will contain T, number of testcases. Then the testcases follow.
Each testcase contains a single line of input, two integers a,b.
## Output Format
For each testcase, output in a single line, answer 1 for bullet, 2 for blitz, 3 for rapid, and 4 for classical format.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	   int a,b;
	   cin>>a>>b;
	   if(a+b < 3)
	   {
	       cout<<1<<endl;
	   }
	   else if(a+b >= 3 && a+b <= 10)
	   {
	       cout<<2<<endl;
	   }
	   else if(a+b >= 11 && a+b <= 60)
	   {
	       cout<<3<<endl;
	   }
	   else
	   {
	       cout<<4<<endl;
	   }
	}
	return 0;
}
```