# First and Last Digit
## Problem
If Give an integer N . Write a program to obtain the sum of the first and last digits of this number.

## Input Format
The first line contains an integer T, the total number of test cases. Then follow T lines, each line contains an integer N.

## Output Format
For each test case, display the sum of first and last digits of N in a new line.

```cpp
#include <iostream>
using namespace std;
typedef long long ll;

int main() {
	ll t;
	cin>>t;
	while(t--)
	{
		ll n,last,first;
		cin>>n;
		last=n%10;
		while(n>=10)
		{
			n=n/10;
		}
		first=n;
		cout<<last+first<<"\n";
		
	}
	return 0;
}
```