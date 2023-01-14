# Genes
## Problem
People in Chefland have three different eye colors, namely brown, blue, and green. green is the rarest of the eye colors whereas brown is most common.

The eye color of the child of two people is most likely to be the most common eye color between them.

You are given two characters denoting the eye colors of two people in Chefland. The character R denotes bRown color, B denotes Blue color, and G denotes Green color.

Determine the most likely eye color of their child. (Print R, B or G denoting bRown, Blue or Green respectively).

Please see the sample test cases below for explained examples.

## Input Format
The first (and only) line of input contains two space-separated characters, the eye colors of the parents.
## Output Format
Print a single character denoting the most likely eye color of the child. (Print R, B or G denoting brown, blue or green respectively).
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	char a,b;
	cin>>a>>b;
	if((a=='R') || (b=='R'))
	{
	    cout<<"R"<<endl;
	}
	else if((a=='B') || (b=='B'))
	{
	    cout<<"B"<<endl;
	}
	else
	{
	    cout<<"G"<<endl;
	}
	return 0;
}

```