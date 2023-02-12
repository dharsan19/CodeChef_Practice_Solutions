# Lucky Four
## Problem
Read problems statements in Mandarin Chinese and Russian.

You are given a list of T integers, for each of them you have to calculate the number of occurrences of the digit 4 in the decimal representation.

## Input
The first line of input consists of a single integer T, denoting the number of integers in the list.

Then, there are T lines, each of them contain a single integer from the list.

## Output
Output T lines. Each of these lines should contain the number of occurrences of the digit 4 in the respective integer from the list.

```cpp
#include <iostream>
using namespace std;

#define ll long long

int main() {
	// your code goes here
	ll t, n;
	cin >> t;
	while (t--) {
	    cin >> n;
	    ll count = 0;
	    while (n > 0) {
	        int mod = n % 10;
	        if (mod == 4) count++;
	        n /= 10;
	    }
	    cout << count << '\n';
	}
	
	return 0;
}
```