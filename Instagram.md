# Instagram
## Problem
Chef categorises an instagram account as spam, if, the following count of the account is more than 1010 times the count of followers.

Given the following and follower count of an account as XX and YY respectively, find whether it is a spam account.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of two space-separated integers XX and YY — the following and follower count of an account, respectively.
## Output Format
For each test case, output on a new line, YES, if the account is spam and NO otherwise.

You may print each character of the string in uppercase or lowercase. For example, the strings YES, yes, Yes and yES are identical.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int following,followers;
	    cin>>following>>followers;
	    if(following>(followers*10))
	    {
	        cout<<"YES"<<endl;
	    }
	    else
	    {
	        cout<<"NO"<<endl;
	    }
	}
	return 0;
}
```