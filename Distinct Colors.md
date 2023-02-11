# Distinct Colors
## Problem
There are N different types of colours numbered from 1 to N. Chef has A i balls having colour i, (1≤i≤N).

Chef will arrange some boxes and put each ball in exactly one of those boxes.
Find the minimum number of boxes Chef needs so that no box contains two balls of same colour.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases. The description of the test cases follows.
The first line of each test case contains a single integer N, denoting the number of colors.
The second line of each test case contains N space-separated integers A 1,A 2,…,A N — denoting the number of balls having colour i.
## Output Format
For each test case, output the minimum number of boxes required so that no box contains two balls of same colour.

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
	    int arr[n],max= 0 ;
	    for(int i = 0;i<n;i++)
	    {
	        cin>>arr[i];
	        if(arr[i] > max)
	        {
	            max = arr[i];
	        }
	    }
	    cout<<max<<endl;
	}
	return 0;
}
```