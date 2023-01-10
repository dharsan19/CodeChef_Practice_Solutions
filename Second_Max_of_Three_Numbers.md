# Second Max of Three Numbers
## Problem
Problem Statement
Write a program that accepts sets of three numbers, and prints the second-maximum number among the three.

## Input
First line contains the number of triples, N.
The next N lines which follow each have three space separated integers.
## Output
For each of the N triples, output one new line which contains the second-maximum integer among the three.
```cpp
#include <iostream>
#include <climits>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int max = INT_MIN, secondmax = INT_MIN;
	    for(int i = 0; i<=2; i++)
	    {
    	    int num;
    	    cin>>num;
    	    if(num>=max)
    	    {
    	        secondmax = max;
    	        max = num;
    	    }
    	    else if (num>secondmax && num != max){
    	        secondmax = num;
    	    }
	    }
	    cout<<secondmax<<endl;
	}
	return 0;
}
```