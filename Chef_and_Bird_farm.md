# Chef and Bird farm
## Problem
In Chefland, each chicken has X legs and each duck has Y legs. Chef's farm can have exactly one type of bird.

Given that the birds on the farm have a total of Z legs:

Print CHICKEN, if the farm can have only chickens but not ducks.
Print DUCK, if the farm can have only ducks but not chickens.
Print ANY, if the farm can have either chickens or ducks.
Print NONE, if the farm can have neither chickens nor ducks.
## Input Format
The first line will contain T, the number of test cases. Then the test cases follow.
Each test case consists of a single line of input, containing three space-separated integers X,Y,Z.
## Output Format
For each test case, output in a single line the type of bird on the farm.

Print CHICKEN, if the farm can have only chickens but not ducks.
Print DUCK, if the farm can have only ducks but not chickens.
Print ANY, if the farm can have either chickens or ducks.
Print NONE, if the farm can have neither chickens nor ducks.
You may print each character of the string in uppercase or lowercase (for example, the strings AnY, anY, any and ANY will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int chicken,duck,legs;
	    cin>>chicken>>duck>>legs;
	    if(legs%chicken == 0 && legs%duck != 0)
	    {
	        cout<<"CHICKEN"<<endl;
	    }
	    else if(legs%chicken != 0 && legs%duck == 0)
	    {
	        cout<<"DUCK"<<endl;
	    }
	    else if(legs%chicken == 0 && legs%duck == 0)
	    {
	        cout<<"ANY"<<endl;
	    }
	    else
	    {
	        cout<<"NONE"<<endl;
	    }
	}
	return 0;
}
```