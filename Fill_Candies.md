# Fill Candies
## Problem
Chef received N candies on his birthday. He wants to put these candies in some bags. A bag has K pockets and each pocket can hold at most M candies. Find the minimum number of bags Chef needs so that he can put every candy into a bag.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of a single line containing three space-separated integers N,K,M.
## Output Format
For each test case, print the minimum number of bags Chef needs so that he can put all the candies in one of the bags.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int candies,pockets,hold;
	    cin>>candies>>pockets>>hold;
	    if(candies%(pockets*hold) == 0)
	    {
	        cout<<candies/(pockets*hold)<<endl;
	    }
	    else
	    {
	        cout<<(candies/(pockets*hold))+1<<endl;
	    }
	}
	return 0;
}
```