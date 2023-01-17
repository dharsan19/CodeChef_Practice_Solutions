# Discount
## Problem
Alice buys a toy with a selling price of 100 rupees. There is a discount of x percent on the toy. Find the amount Alice needs to pay for it.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
The first and only line of each test case contains a single integer, x — the discount on the toy.
## Output Format
For each test case, output on a new line the price that Alice needs to pay.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int discount,price;
	    cin>>discount;
	    price = 100 - discount;
	    cout<<price<<endl;
	}
	return 0;
}
```