# TV Discount
## Problem
Chef is looking to buy a TV and has shortlisted two models. The first one costs A rupees, while the second one costs B rupees.

Since there is a huge sale coming up on Chefzon, Chef can get a flat discount of C rupees on the first TV, and a flat discount of D rupees on the second one.

Help Chef determine which of the two TVs would be cheaper to buy during the sale.

## Input Format
The first line contains a single integer T — the number of test cases. Then the test cases follow.
The first and only line of each test case contains four space-separated integers A, B, C and D — the marked price (in rupees) of the first TV, the marked price (in rupees) of the second TV, the flat discount (in rupees) of the first TV, and the flat discount (in rupees) of the second TV.
## Output Format
For each test case, print a single line containing the string First if the first TV is cheaper to buy with discount, or Second if the second TV is cheaper to buy with discount. If both of them cost the same after discount, print Any.

You may print each character of the string in uppercase or lowercase (for example, the strings first, First, fIRSt, and FIRST will all be treated as identical).
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    float tv1,tv2,dis1,dis2;
	    cin>>tv1>>tv2>>dis1>>dis2;
	    float price1, price2;
	    price1 = tv1 - dis1;
	    price2 = tv2 - dis2;
	    if(price1 < price2)
	    {
	        cout<<"First"<<endl;
	    }
	    else if(price2 < price1)
	    {
	        cout<<"Second"<<endl;
	    }
	    else
	    {
	        cout<<"Any"<<endl;
	    }
	}
	return 0;
}
```