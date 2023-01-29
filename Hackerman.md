# Hackerman
## Problem
Hackerman wants to know who is the better player between Bob and Alice with the help of a game.

The game proceeds as follows:

First, Alice throws a die and gets the number A
Then, Bob throws a die and gets the number B
Alice wins the game if the sum on the dice is a prime number; and Bob wins otherwise.
Given A and B, determine who wins the game.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
The first and only line of each test case contains two space-separated integers A and B.
## Output Format
For each test case, output on a new line the winner of the game: Alice or Bob.

Each letter of the output may be printed in either uppercase or lowercase, i.e, Alice, ALICE, AlIce and aLIcE will all be considered equivalent.

```cpp
#include <iostream>
using namespace std;

bool isprime(int n)
{
    if(n <= 1)
        return false; 
        
    for(int i = 2; i < n; i++)
    {
        if(n % i == 0)
            return false;
    }

    return true;

}

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b;
	    cin>>a;
	    cin>>b;
	    isprime(a+b) ? cout<<"Alice\n" : cout<<"Bob\n" ;
	}
	return 0;
}
```