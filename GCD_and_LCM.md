# GCD and LCM
## Problem
Two integers A and B are the inputs. Write a program to find GCD and LCM of A and B.

## Input Format
The first line contains an integer T, total number of testcases. Then follow T lines, each line contains an integer A and B.

## Output Format
Display the GCD and LCM of A and B separated by space respectively. The answer for each test case must be displayed in a new line.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    long int a,b,lcm,gcd;
	    cin>>a>>b;
	    long int temp1 = a, temp2 = b;
        while(temp1 != temp2)
        {
            if(temp1 > temp2)
            {
                temp1 -= temp2;
            }
            else
            {
                temp2 -= temp1;
            }
        }
        gcd = temp1;
	    lcm = a*b /gcd;
	    cout<<gcd<<" "<<lcm<<endl;
	}
	return 0;
}
```