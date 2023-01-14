# Wordle
## Problem
Chef invented a modified wordle.

There is a hidden word SS and a guess word TT, both of length 55.

Chef defines a string MM to determine the correctness of the guess word.

## Input Format
First line will contain TT, number of test cases. Then the test cases follow.
Each test case contains of two lines of input.
First line contains the string SS - the hidden word.
Second line contains the string TT - the guess word.
## Output Format
For each test case, print the value of string MM.

You may print each character of the string in uppercase or lowercase (for example, the strings \texttt{BgBgB}BgBgB, \texttt{BGBGB}BGBGB, \texttt{bgbGB}bgbGB and \texttt{bgbgb}bgbgb will all be treated as identical).
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    string str1,str2,str3;
	    cin>>str1>>str2;
	    for(int i=0;i<5;i++)
	    {
	        if(str1[i] == str2[i]){
	            str3.append("G");}
	        else{
	            str3.append("B");}
	    }
	    cout<<str3<<endl;
	}
	return 0;
}

```