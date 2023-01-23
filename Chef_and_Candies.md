# Chef and Candies
## Problem
There are N children and Chef wants to give them 1 candy each. Chef already has X candies with him. To buy the rest, he visits a candy shop. In the shop, packets containing exactly 4 candies are available.

Determine the minimum number of candy packets Chef must buy so that he is able to give 1 candy to each of the N children.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
The first and only line of each test case contains two integers N and X — the number of children and the number of candies Chef already has.
## Output Format
For each test case, output the minimum number of candy packets Chef must buy so that he is able to give 1 candy to each of the N children.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,x,ans;
	    cin>>n>>x;
        if((n-x)%4 == 0 && n > x)
        {
            cout<<(n-x)/4<<endl;
        }
        else if(n <= x)
        {
            cout<<0<<endl;
        }
        else 
        {
            cout<<((n-x)/4)+1<<endl;
        }
	}
    return 0;
}
```