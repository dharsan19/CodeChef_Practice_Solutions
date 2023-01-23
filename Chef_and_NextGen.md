# Chef and NextGen
## Problem
Chef is currently working for a secret research group called NEXTGEN. While the rest of the world is still in search of a way to utilize Helium-3 as a fuel, NEXTGEN scientists have been able to achieve 2 major milestones:

Finding a way to make a nuclear reactor that will be able to utilize Helium-3 as a fuel
Obtaining every bit of Helium-3 from the moon's surface
Moving forward, the project requires some government funding for completion, which comes under one condition: to prove its worth, the project should power Chefland by generating at least A units of power each year for the next B years.

Help Chef determine whether the group will get funded assuming that the moon has X grams of Helium-3 and 1 gram of Helium-3 can provide Y units of power.

## Input Format
The first line of input contains an integer T, the number of testcases. The description of T test cases follows.
Each test case consists of a single line of input, containing four space-separated integers A,B,X,Y respectively.
## Output Format
For each test case print on a single line the answer — Yes if NEXTGEN satisfies the government's minimum requirements for funding and No otherwise.

You may print each character of the answer string in either uppercase or lowercase (for example, the strings "yEs", "yes", "Yes" and "YES" will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,x,y;
	    cin>>a>>b>>x>>y;
	    if(a*b <= x*y)
	    {
	        cout<<"Yes"<<endl;
	    }
	    else
	    {
	        cout<<"No"<<endl;
	    }
	}
	return 0;
}
```