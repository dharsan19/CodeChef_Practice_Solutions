# Complementary Strand in a DNA
## Problem
You are given the sequence of Nucleotides of one strand of DNA through a string S of length N. 
S contains the character A,T,C, and G only.

Chef knows that:

A is complementary to T.
T is complementary to A.
C is complementary to G.
G is complementary to C.
Using the string S, determine the sequence of the complementary strand of the DNA.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
First line of each test case contains an integer N - denoting the length of string S.
Second line contains N characters denoting the string S.
## Output Format
For each test case, output the string containing N characters - sequence of nucleotides of the complementary strand.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int t1;
	    cin>>t1;
	    char str[t1];
	    cin>>str;
	    for(int i = 0; i < t1; i++)
	    {
	        if(str[i] == 'A')
	        {
	            cout<<'T';
	        }
	        else if(str[i] == 'T')
	        {
	            cout<<'A';
	        }
	        else if(str[i] == 'C')
	        {
	            cout<<'G';
	        }
	        else
	        {
	            cout<<'C';
	        }
	    }
	    cout<<endl;
	}
	return 0;
}
```