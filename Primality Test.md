# Primality Test
## Problem
Alice and Bob are meeting after a long time. As usual they love to play some math games. This times Alice takes the call and decides the game. The game is very simple, Alice says out an integer and Bob has to say whether the number is prime or not. Bob as usual knows the logic but since Alice doesn't give Bob much time to think, so Bob decides to write a computer program.

Help Bob accomplish this task by writing a computer program which will calculate whether the number is prime or not .

## Input
The first line of the input contains an integer T, the number of testcases. T lines follow.

Each of the next T lines contains an integer N which has to be tested for primality.

## Output
For each test case output in a separate line, "yes" if the number is prime else "no."

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int num,prime = 1;
	    cin>>num;
        for(int i =2;i<num;i++)
        {
            if((num%i)==0)
            {
                prime = 0;
            }
        }
        if(num == 1 || num == 0)
        {
            cout<<"no"<<endl;
        }
        else if(prime == 1)
        {
            cout<<"yes"<<endl;
        }
        else
        {
            cout<<"no"<<endl;
        }
	}
	return 0;
}
```