# Maximise the Tastiness
## Problem
Chef is making a dish that consists of exactly two ingredients. He has four ingredients A,B,C and D with tastiness a,b,c, and d respectively. He can use either A or B as the first ingredient and either C or D as the second ingredient.

The tastiness of a dish is the sum of tastiness of its ingredients. Find the maximum possible tastiness of the dish that the chef can prepare.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
The first and only line of each test case contains four space-separated integers a,b,c, and d — the tastiness of the four ingredients.
## Output Format
For each test case, output on a new line the maximum possible tastiness of the dish that chef can prepare.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,c,d;
	    cin>>a>>b>>c>>d;
	    cout<<max(a,b) + max(c,d)<<endl;
	}
	return 0;
}
```