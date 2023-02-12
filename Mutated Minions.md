# Mutated Minions
## Problem
Gru has not been in the limelight for a long time and is, therefore, planning something particularly nefarious. Frustrated by his minions' incapability which has kept him away from the limelight, he has built a transmogrifier — a machine which mutates minions.

Each minion has an intrinsic characteristic value (similar to our DNA), which is an integer. The transmogrifier adds an integer K to each of the minions' characteristic value.

Gru knows that if the new characteristic value of a minion is divisible by 7, then it will have Wolverine-like mutations.

Given the initial characteristic integers of N minions, all of which are then transmogrified, find out how many of them become Wolverine-like.

## Input Format
The first line contains one integer, T, which is the number of test cases.
Each test case contains of 2 lines of input.

The first line contains two integers N and K, as described in the statement
The next line contains N integers, which denote the initial characteristic values for the minions
## Output Format
For each testcase, output one integer in a new line, which is the number of Wolverine-like minions after the transmogrification.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,k;
	    cin>>n>>k;
	    int arr[n],count = 0;
	    for(int i =0; i<n; i++)
	    {
	        cin>>arr[i];
	        arr[i] = arr[i]+k;
	        if(arr[i]%7 == 0)
	        {
	            count++;
	        }
	    }
	    cout<<count<<endl;
	}
	return 0;
}
```