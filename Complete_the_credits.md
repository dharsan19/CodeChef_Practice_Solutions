# Complete the credits
## Problem
In Uttu's college, a semester is said to be a:

Overload semester if the number of credits taken \gt 65>65.
Underload semester if the number of credits taken \lt 35<35.
Normal semester otherwise
Given the number of credits XX taken by Uttu, determine whether the semester is Overload, Underload or Normal.

## Input Format
The first line will contain TT - the number of test cases. Then the test cases follow.
The first and only of each test case contains a single integer XX - the number of credits taken by Uttu.
You may print each character of Overload, Underload and Normal in uppercase or lowercase (for example, ovErLoAd, oVERlOAD, OVERLOAD will be considered identical).

## Output Format
For each test case, output Overload, Underload or Normal depending upon the number of credits taken by Uttu.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x;
	    cin>>x;
	    if(x>65)
	    {
	        cout<<"Overload"<<endl;
	    }
	    else if(x<35)
	    {
	        cout<<"Underload"<<endl;
	    }
	    else
	    {
	        cout<<"Normal"<<endl;
	    }
	}
	return 0;
}
```