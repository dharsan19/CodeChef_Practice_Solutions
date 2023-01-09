# Chef and Brain Speed
## Problem
In ChefLand, human brain speed is measured in bits per second (bps). Chef has a threshold limit of XX bits per second above which his calculations are prone to errors. If Chef is currently working at YY bits per second, is he prone to errors?

If Chef is prone to errors print YES, otherwise print NO.

## Input Format
The only line of input contains two space separated integers XX and YY — the threshold limit and the rate at which Chef is currently working at.

## Output Format
If Chef is prone to errors print YES, otherwise print NO.

You may print each character of the string in uppercase or lowercase (for example, the strings yes, Yes, yEs, and YES will all be treated as identical).
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int x,y;
	cin>>x>>y;
	if(y>x)
	    cout<<"YES"<<endl;
    else
        cout<<"NO"<<endl;
	return 0;
}
```