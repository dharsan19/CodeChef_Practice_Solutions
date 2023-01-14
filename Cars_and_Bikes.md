# Cars and Bikes
## Problem
Chef opened a company which manufactures cars and bikes. Each car requires 44 tyres while each bike requires 22 tyres. Chef has a total of NN tyres (NN is even). He wants to manufacture maximum number of cars from these tyres and then manufacture bikes from the remaining tyres.

Chef's friend went to Chef to purchase a bike. If Chef's company has manufactured even a single bike then Chef's friend will be able to purchase it.

Determine whether he will be able to purchase the bike or not.

## Input Format
The first line contains an integer TT denoting the number of test cases. The TT test cases then follow.
The first line of each test case contains an integer NN denoting the number of tyres.
## Output Format
For each test case, output YES or NO depending on whether Chef's friend will be able to purchase the bike or not. Output is case insensitive.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n;
	    cin>>n;
	    if((n%4)>=2)
	    {
	        cout<<"YES"<<endl;
	    }
	    else if(n==2)
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