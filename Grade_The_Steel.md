# Grade The Steel
## Problem
A certain type of steel is graded according to the following conditions.

Hardness of the steel must be greater than 50
Carbon content of the steel must be less than 0.7
Tensile strength must be greater than 5600
The grades awarded are as follows:

Grade is 10 if all three conditions are met
Grade is 9 if conditions (1) and (2) are met
Grade is 8 if conditions (2) and (3) are met
Grade is 7 if conditions (1) and (3) are met
Grade is 6 if only one condition is met
Grade is 5 if none of the three conditions are met
Write a program to display the grade of the steel, based on the values of hardness, carbon content and tensile strength of the steel, given by the user.

## Input Format
The first line contains an integer T, total number of testcases. Then follow T lines, each line contains three numbers hardness, carbon content and tensile strength of the steel.

## Output Format
For each test case, print Grade of the steel depending on Conditions, in a new line.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    float a,b,c;
	    cin>>a>>b>>c;
	    if((a>50) && (b<0.7) && (c>5600))
	    {
	        cout<<10<<endl;
	    }
	    else if((a>50) && (b<0.7)) 
	    {
	        cout<<9<<endl;
	    }
	    else if((b<0.7) && (c>5600)) 
	    {
	        cout<<8<<endl;
	    }
	    else if((a>50) && (c>5600)) 
	    {
	        cout<<7<<endl;
	    }
	    else if((a>50) || (b<0.7) || (c>5600)) 
	    {
	        cout<<6<<endl;
	    }
	    else 
	    {
	        cout<<5<<endl;
	    }
	}
	return 0;
}

```