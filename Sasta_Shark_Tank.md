# Sasta Shark Tank
## Problem
Devendra just had a million-dollar idea and he needs funds to startup. He was recently invited to Sasta Shark Tank (A TV show where entrepreneurs pitch their ideas to investors hoping to get investment in return).

He was offered deals from two investors. The first investor offers A dollars for 10% of his company and the second investor offers B dollars for 20% of his company. Devendra will accept the offer from the investor whose valuation of the company is more. Determine which offer will Devendra accept or if both the offers are equally good.

For example, if the first investor offers 300 dollars for 10% of the company, then the first investor's valuation of the company is 3000 dollars since 10% of 3000=300. If the second investor offers 500 dollars for 20% of the company, then the second investor's valuation of the company is 2500 dollars since 20% of 2500=500.

## Input Format
The first line contains a single integer T - the number of test cases. Then the test cases follow.
The first and only line of each test case contains two integers A and B - the amount offered by first investor for 10% of Devendra's company and the amount offered by second investor for 20% of Devendra's company respectively.
## Output Format
For each test case, Output FIRST if Devendra should accept the first investor's deal, output SECOND if he should accept the second investor's deal, otherwise output ANY if both deals are equally good.

You may print each character of the strings in uppercase or lowercase (for example, the strings "FiRst", "First", "FIRST", and "FIrst" will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int investor1,investor2;
	    cin>>investor1>>investor2;
	    if(investor1*10 == investor2*5)
	    {
	        cout<<"ANY"<<endl;
	    }
	    else if(investor1*10 > investor2*5)
	    {
	        cout<<"FIRST"<<endl;
	    }
	    else
	    {
	        cout<<"SECOND"<<endl;
	    }
	}
	return 0;
}
```