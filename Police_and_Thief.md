# Police and Thief
## Problem
Chef discovered that his secret recipe has been stolen. He immediately informs the police of the theft.

It is known that the policeman and thief move on the number line. You are given that:

The initial location of the policeman on the number line is X and his speed is 2 units per second.
The initial location of the thief on the number line is Y and his speed is 1 unit per second.
Find the minimum time (in seconds) in which the policeman can catch the thief. Note that, the policeman catches the thief as soon as their locations become equal and the thief will try to evade the policeman for as long as possible.

## Input Format
The first line of input will contain an integer T — the number of test cases. The description of T test cases follows.
The first and only line of each test case contains two integers X and Y, as described in the problem statement.
## Output Format
For each test case, output in a single line the minimum time taken by the policeman to catch the thief.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int x,y;
	    cin>>x>>y;
	    int count = 0;
        if( x > y)
        {
            while(1)
            {
                if( x <= y)
                {
                    break;
                }
                x -= 2;
                y -= 1;
                count++;
            }
        }
        else
        {
            while(1)
            {
                if(x >= y)
                {
                    break;
                }
                x += 2;
                y += 1;
                count++;
            }
        }
	    cout<<count<<endl;
	}
	return 0;
}
```