# Mario and the Broken String
## Problem
Mario was going to gift Princess Peach a string S of even length N.

Mario was clumsy and thus, broke the string in the middle. He now has two strings A and B such that A=S[1, 2N ] and B=S[ N +1,N].

Mario is not sure about the order in which he should join the strings A and B to get the string S. Thus, he joins the strings in any random order. Find whether it is guaranteed that Mario will get the same string S if he joins the strings A and B in any order.

Note that S[L,R] denotes a substring of string S starting at index L and having a length (R−L+1).

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of two lines of input:
The first line of each test case contains N - the length of the initial string S.
The second line contains the string S.
## Output Format
For each test case, print YES if it is guaranteed that Mario will get the same string S irrespective of the order in which he joins the strings A and B and NO otherwise.

You may print each character of the string in uppercase or lowercase (for example, the strings YES, yEs, yes, and yeS will all be treated as identical).

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,count = 0;
	    cin>>n;
	    char arr[n];
	    for(int i = 0; i<n; i++)
	    {
	        cin>>arr[i];
	    }
	    for(int i = 0; i<n/2; i++)
	    {
	        if(arr[i] == arr[(n/2)+i])
	        {
	            count++;
	        }
	    }
	    if(count == n/2)
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