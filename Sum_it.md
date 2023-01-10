# Sum it
## Problem
Bob received an assignment from his school: he has two numbers AA and BB, and he has to find the sum of these two numbers.
Alice, being a good friend of Bob, told him that the answer to this question is CC.
Bob doesn't completely trust Alice and asked you to tell him if the answer given by Alice is correct or not.
If the answer is correct print "YES", otherwise print "NO" (without quotes).

## Input Format
The first line of input will contain a single integer TT, denoting the number of test cases.
The first and only line of each test case consists of three space-separated integers A, B,A,B, and CC.
## Output Format
For each test case, output on a new line the answer: YES if Alice gave the right answer, and NO otherwise.

Each character of the output may be printed in either uppercase or lowercase, i.e, the outputs Yes, YES, yEs and yes will be treated as equivalent.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,c;
	    cin>>a>>b>>c;
	    if((a+b)==c)
	    {
	        cout<<"YES"<<endl;
	    }
	    else
	    {
	        cout<<"NO"<<endl;
	    }
	}
	return 0;
}
```