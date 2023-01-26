# Chef Drinks Tea
## Problem
Chef has planned that he will drink exactly X liters of tea daily. He has an empty jar having a capacity of Y liters.

Chef can visit the tea shop to refill the jar. In each refill, the jar is completely filled to the brim and Chef is charged Z rupees.

Chef wonders what is the minimum amount of money he has to pay for drinking exactly X liters of tea daily.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains of a single line of input, three space-separated integers X, Y, and Z denoting the amount of tea Chef has to drink daily, the capacity of his jar and the cost of refilling his jar.
## Output Format
For each test case, output in a single line, the minimum amount Chef has to pay.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y,z;
	    cin>>x>>y>>z;
        if(x%y == 0)
        {
            cout<<(x/y)*z<<endl;
        }
        else
        {
            cout<<((x/y)+1)*z<<endl;
        }
	}
	return 0;
}

```