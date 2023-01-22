# Odd Sum Pair
## Problem
Chef has 3 numbers A,B and C.

Chef wonders if it is possible to choose exactly two numbers out of the three numbers such that their sum is odd.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of three integers A,B,C.
## Output Format
For each test case, output YES if you can choose exactly two numbers with odd sum, NO otherwise.

The output is case-insensitive. Thus, the strings YES, yes, yeS, and Yes are all considered the same.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
    {
        int arr[3],count = 0;
        for(int i=0; i<3; i++)
        {
            cin>>arr[i];
            if(arr[i]%2 == 0)
            {
                count++;
            }
        }
        if(count ==1 || count == 2)
        {
            cout<<"YES"<<endl;
        }
        else
        {
            cout<<"NO"<<endl;
        }
    }
	return 0;
}
```