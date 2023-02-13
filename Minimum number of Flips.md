# Minimum number of Flips
## Problem
Chef has an array A of length N consisting of 1 and −1 only.

In one operation, Chef can choose any index (1≤i≤N) and multiply the element A i by −1.

Find the minimum number of operations required to make the sum of the array equal to 0. Output -1 if the sum of the array cannot be made 0.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
First line of each test case consists of a single integer N denoting the length of the array.
Second line of each test case contains N space-separated integers A 1,A 2,…,A N denoting the array A.
## Output Format
For each test case, output the minimum number of operations to make the sum of the array equal to 0. Output -1 if it is not possible to make the sum equal to 0.

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
	    int arr[n],sum = 0;
	    for(int i = 0; i<n; i++)
	    {
	        cin>>arr[i];
	        sum += arr[i];
	    }
	    if(n%2 == 0)
	    {
            cout<<abs(sum)/2<<endl;        
	    }
	    else
	    {
	        cout<<-1<<endl;
	    }
	}
	return 0;
}
```