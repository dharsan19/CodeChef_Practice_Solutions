# Sugarcane Juice Business
## Problem
While Alice was drinking sugarcane juice, she started wondering about the following facts:

The juicer sells each glass of sugarcane juice for 50 coins.
He spends 20% of his total income on buying sugarcane.
He spends 20% of his total income on buying salt and mint leaves.
He spends 30% of his total income on shop rent.
Alice wonders, what is the juicer's profit (in coins) when he sells N glasses of sugarcane juice?

## Input Format
The first line of input will contain an integer T — the number of test cases. The description of T test cases follows.
The first and only line of each test case contains an integer N, as described in the problem statement.
## Output Format
For each test case, output on a new line the juicer's profit when he sells N glasses of juice.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,ans;
	    cin>>n;
	    ans = n*15;
	    cout<<ans<<endl;
	}
	return 0;
}
```