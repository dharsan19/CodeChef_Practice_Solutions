# Gross Salary
## Problem
In a company an emplopyee is paid as under: If his basic salary is less than Rs. 1500, then HRA = 10% of base salary and DA = 90% of basic salary.
If his salary is either equal to or above Rs. 1500, then HRA = Rs. 500 and DA = 98% of basic salary. If the Employee's salary is input, write a program to find his gross salary.

NOTE: Gross Salary = Basic Salary + HRA + DA

## Input
The first line contains an integer T, total number of testcases. Then follow T lines, each line contains an integer salary.

## Output
For each test case, output the gross salary of the employee in a new line. Your answer will be considered correct if the absolute error is less than 10-2.
```cpp
#include <iostream>
#include <iomanip>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    double basic,hra,da,gross;
	    cin>>basic;
	    if(basic<1500)
	    {
	        hra = (basic/100)*10;
	        da = (basic/100)*90;
	        gross = basic+hra+da;
	        //printing upto 2 decimal points using printf statements
	        printf("%.2f\n",gross);
	    }
	    else
	    {
	        hra = 500;
	        da = (basic/100)*98;
	        //printing upto 2 decimal points using setprecision by including iomanip header
	        cout<<fixed<<setprecision(2)<<basic+hra+da<<endl;
	    }
	}
	return 0;
}
```