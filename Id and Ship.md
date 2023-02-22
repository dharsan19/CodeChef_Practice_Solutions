# Id and Ship
## Problem
Write a program that takes in a letterclass ID of a ship and display the equivalent string class description of the given ID. Use the table below.

Class ID	Ship Class
B or b	BattleShip
C or c	Cruiser
D or d	Destroyer
F or f	Frigate
## Input Format
The first line contains an integer T, the total number of testcases. Then T lines follow, each line contains a character.

## Output Format
For each test case, display the Ship Class depending on ID, in a new line.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    char c;
	    cin>>c;
	    if(c == 'b' || c == 'B')
	    {
	        cout<<"BattleShip"<<endl;
	    }
	    else if(c == 'c' || c == 'C')
	    {
	        cout<<"Cruiser"<<endl;
	    }
	    else if(c == 'd' || c == 'D')
	    {
	        cout<<"Destroyer"<<endl;
	    }
	    else
	    {
	        cout<<"Frigate"<<endl;
	    }
	}
	return 0;
}
```