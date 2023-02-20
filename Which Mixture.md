# Which Mixture
## Problem
Read problem statements in Bengali, Mandarin Chinese, Russian, and Vietnamese as well.
Chef has A units of solid and B units of liquid. He combines them to create a mixture. What kind of mixture does Chef produce: a solution, a solid, or a liquid?

A mixture is called :

A solution if A>0 and B>0,

A solid if B=0, or

A liquid if A=0.

## Input Format
The first line contains T denoting the number of test cases. Then the test cases follow.
Each test case contains two space-separated integers A and B on a single line.
## Output Format
For each test case, output on a single line the type of mixture Chef produces, whether it is a Solution, Solid, or Liquid. The output is case sensitive.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b;
	    cin>>a>>b;
	    if(a>0 && b>0)
	    {
	        cout<<"Solution"<<endl;
	    }
	    else if( b == 0 && a>0)
	    {
	        cout<<"Solid"<<endl;
	    }
	    else
	    {
	        cout<<"Liquid"<<endl;
	    }
	}
	return 0;
}
```