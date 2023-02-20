# Body Mass Index
## Problem
Read problems statements in Hindi, Mandarin Chinese, Vietnamese, and Bengali as well.
You are given the height H (in metres) and mass M (in kilograms) of Chef. The Body Mass Index (BMI) of a person is computed as m/H 2 .

Report the category into which Chef falls, based on his BMI:

Category 1: Underweight if BMI ≤18
Category 2: Normal weight if BMI ∈{19, 20,…, 24}
Category 3: Overweight if BMI ∈{25, 26,…, 29}
Category 4: Obesity if BMI ≥30
## Input:

The first line of input will contain an integer, T, which denotes the number of testcases. Then the testcases follow.
Each testcase contains a single line of input, with two space separated integers, M,H, which denote the mass and height of Chef respectively.
## Output: 
For each testcase, output in a single line, 1,2,3 or 4, based on the category in which Chef falls.

```cpp
#include <iostream>
#include <cmath>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int m,h;
	    cin>>m>>h;
	    int bmi = m/pow(h,2);
	    if(bmi <= 18)
	    {
	        cout<<1<<endl;
	    }
	    else if(bmi >=19 && bmi <=24)
	    {
	        cout<<2<<endl;
	    }
	    else if(bmi >=25 && bmi <= 29)
	    {
	        cout<<3<<endl;
	    }
	    else
	    {
	        cout<<4<<endl;
	    }
	}
	return 0;
}
```