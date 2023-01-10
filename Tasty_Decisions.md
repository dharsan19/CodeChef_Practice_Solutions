# Tasty Decisions
## Problem
Chef is buying sweet things to prepare for Halloween!

The shop sells both chocolate and candy.

Each bar of chocolate has a tastiness of XX.
Each piece of candy has a tastiness of YY.
One packet of chocolate contains 22 bars, while one packet of candy contains 55 pieces.

Chef can only buy one packet of something sweet, and so has to make a decision: which one should he buy in order to maximize the total tastiness of his purchase?

Print Chocolate if the packet of chocolate is tastier, Candy if the packet of candy is tastier, and Either if they have the same tastiness.

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of one line of input, containing two space-separated integers XX and YY — the tastiness of one bar of chocolate and one piece of candy, respectively.
## Output Format
For each test case, output on a new line the answer:

Chocolate if the packet of chocolate is tastier.
Candy if the packet of candy is tastier.
Either if they have the same tastiness.
You may print each character of the output in either uppercase or lowercase, i.e, Candy, CANDY, CaNdY and cANDy will all be treated as equivalent.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int chocolate, candy;
	    cin>>chocolate>>candy;
	    if((chocolate*2)>(candy*5))
	    {
	        cout<<"Chocolate"<<endl;
	    }
	    else if((chocolate*2)<(candy*5))
	    {
	        cout<<"Candy"<<endl;
	    }
	    else
	    {
	        cout<<"Either"<<endl;
	    }
	}
	return 0;
}
```