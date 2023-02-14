# Economics Class
## Problem
Alice has recently learned in her economics class that the market is said to be in equilibrium when the supply is equal to the demand.

Alice has market data for N time points in the form of two integer arrays S and D. Here, S i  denotes the supply at the th  point of time and D i  denotes the demand at the i th point of time, for each 1≤i≤N.

Help Alice in finding out the number of time points at which the market was in equilibrium.

## Input Format
The first line of input will contain an integer T — the number of test cases. The description of T test cases follows.
Each test case contains three lines of input.
The first line of each test case contains an integer N, the length of the arrays S and D.
The second line of each test case contains N space-separated integers S 1 ,S 2 ,…,S N.
The third line of each test case contains N space-separated integers D 1,D 2,…,D N.
## Output Format
For each test case, output the number of time points at which the market was in equilibrium.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,count = 0;
	    cin>>n;
	    int arr[n],arr1[n];
	    for(int i =0; i<n; i++)
	    {
	        cin>>arr[i];
	    }
	    for(int i =0; i<n; i++)
	    {
	        cin>>arr1[i];
	    }
	    for(int i = 0; i<n; i++)
	    {
	        if(arr[i] == arr1[i]){
	            count++;
	        }
	    }
	    std::cout << count << std::endl;
	}
	return 0;
}
```