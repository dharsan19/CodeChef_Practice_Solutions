# Water Mixing
## Problem
Chef is setting up a perfect bath for himself. He has X litres of hot water and Y litres of cold water.
The initial temperature of water in his bathtub is A degrees. On mixing water, the temperature of the bathtub changes as following:

The temperature rises by 1 degree on mixing 1 litre of hot water.
The temperature drops by 1 degree on mixing 1 litre of cold water.
Determine whether he can set the temperature to B degrees for a perfect bath.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of four space-separated integers A,B,X, and Y — the initial temperature of bathtub, the desired temperature of bathtub, the amount of hot water in litres, and the amount of cold water in litres respectively.
## Output Format
For each test case, output on a new line, YES if Chef can get the desired temperature for his bath, and NO otherwise.

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
	    int a,b,x,y;
	    cin>>a>>b>>x>>y;
	    if(a<b)
	    {
	        for(int i = 1; i<=x; i++)
	        {
	            a+=1;
	            if(a == b)
	            {
	                cout<<"YES"<<endl;
	                break;
	            }
	        }
	        if(a!=b)
	            cout<<"NO"<<endl;
	    }
	    else if(a>b)
	    {
	        for(int i =1;i<=y;i++)
	        {
	            a -=1;
	            if(a==b)
	            {
	                cout<<"YES"<<endl;
	                break;
	            }
	        }
	        if(a!=b)
	            cout<<"NO"<<endl;
	    }
	    else
	    {
	        cout<<"YES"<<endl;
	    }
	}
	return 0;
}
```