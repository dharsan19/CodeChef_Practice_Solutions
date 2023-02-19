# Nearest Court
## Problem
Chef and Chefina are at positions X and Y on a number line.

They both love badminton.

It is known that badminton courts are located at every integer point.

They want to find a court such that the maximum distance travelled by either of them is minimized.

Formally, suppose they choose the badminton court at position Z. You need to find the minimum value of max(∣X−Z∣,∣Y−Z∣) across all possible choices of Z. Here, ∣X∣ denotes absolute value of X.

Report this minimum value.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of two space-separated integers X and Y.
## Output Format
For each test case, output the minimum possible value of max(∣X−Z∣,∣Y−Z∣).

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
	    int z = abs(x-y);
	    if(z%2 == 0)
	    {
	        cout<<z/2<<endl;
	    }
	    else
	    {
	        cout<<(z/2)+1<<endl;
	    }
	}
	return 0;
}
``