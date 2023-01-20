# Broken Phone
## Problem
Uttu broke his phone. He can get it repaired by spending X rupees or he can buy a new phone by spending Y rupees. Uttu wants to spend as little money as possible. Find out if it is better to get the phone repaired or to buy a new phone.

## Input Format
The first line contains a single integer T — the number of test cases. Then the test cases follow.
The first and only line of each test case contains two space-separated integers X and Y — the cost of getting the phone repaired and the cost of buying a new phone.
## Output Format
For each test case,

output REPAIR if it is better to get the phone repaired.
output NEW PHONE if it is better to buy a new phone.
output ANY if both the options have the same price.
You may print each character of REPAIR, NEW PHONE and ANY in uppercase or lowercase (for example, any, ANy, Any will be considered identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int repair,new_phone;
	    cin>>repair>>new_phone;
	    if(repair == new_phone)
	    {
	        cout<<"ANY"<<endl;
	    }
	    else if(repair < new_phone)
	    {
	        cout<<"REPAIR"<<endl;
	    }
	    else
	    {
	        cout<<"NEW PHONE"<<endl;
	    }
	}
	return 0;
}
```