# Cost of Groceries
## Problem
Chef visited a grocery store for fresh supplies. There are N items in the store where the i th  item has a freshness value A i  and cost B i .

Chef has decided to purchase all the items having a freshness value greater than equal to X. Find the total cost of the groceries Chef buys.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of multiple lines of input.
The first line of each test case contains two space-separated integers N and X — the number of items and the minimum freshness value an item should have.
The second line contains N space-separated integers, the array A, denoting the freshness value of each item.
The third line contains N space-separated integers, the array B, denoting the cost of each item.
## Output Format
For each test case, output on a new line, the total cost of the groceries Chef buys.

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
	    int arr[n],arr1[n],sum = 0;
	    for(int i = 0; i<n; i++)
	    {
	        cin>>arr[i];
	    }
	    for(int i = 0; i<n; i++)
	    {
	        cin>>arr1[i];
	    }
	    for(int i = 0; i<n; i++)
	    {
	        if(arr[i] >= x)
	        {
	            sum += arr1[i];
	        }
	    }
	    cout<<sum<<endl;
	}
	return 0;
}
```