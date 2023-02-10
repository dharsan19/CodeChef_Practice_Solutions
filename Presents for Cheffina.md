# Presents for Cheffina
## Problem
Chef has fallen in love with Cheffina, and wants to buy N gifts for her. On reaching the gift shop, Chef got to know the following two things:

The cost of each gift is 1 coin.
On the purchase of every 4 th gift, Chef gets the 5 thgift free of cost.
What is the minimum number of coins that Chef will require in order to come out of the shop carrying N gifts?

## Input Format
The first line of input will contain an integer T — the number of test cases. The description of T test cases follows.
The first and only line of each test case contains an integer N, the number of gifts in the shop.
## Output Format
For each test case, output on a new line the minimum number of coins that Chef will require to obtain all N gifts.

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
	    if(n>4)
	        cout<<n-(n/5)<<endl;
	    else
	        cout<<n<<endl;
	}
	return 0;
}
```