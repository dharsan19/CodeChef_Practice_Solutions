# Credit score
## Problem
To access CRED programs, one needs to have a credit score of 750 or more.
Given that the present credit score is X, determine if one can access CRED programs or not.

If it is possible to access CRED programs, output YES, otherwise output NO.

## Input Format
The first and only line of input contains a single integer X, the credit score.

## Output Format
Print YES if it is possible to access CRED programs. Otherwise, print NO.

You may print each character of the string in uppercase or lowercase (for example, the strings YeS, yEs, yes and YES will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int score;
	cin>>score;
	if(score >= 750)
	{
	    cout<<"YES"<<endl;
	}
	else
	{
	    cout<<"NO"<<endl;
	}
	return 0;
}

```