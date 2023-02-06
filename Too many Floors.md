# Too many Floors
## Problem
Chef and Chefina are residing in a hotel.

There are 10 floors in the hotel and each floor consists of 10 rooms.

Floor 1 consists of room numbers 1 to 10.
Floor 2 consists of room numbers 11 to 20.
…
…
Floor i consists of room numbers 10⋅(i−1)+1 to 10⋅i.
You know that Chef's room number is X while Chefina's Room number is Y.
If Chef starts from his room, find the number of floors he needs to travel to reach Chefina's room.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
Each test case contains of a single line of input, two integers X,Y, the room numbers of Chef and Chefina respectively.
## Output Format
For each test case, output the number of floors Chef needs to travel to reach Chefina's room.

```cpp
#include <iostream>
using namespace std;
int main()
{
	int t;
	cin>>t;
	while(t--)
	{
		int x,y;
		cin>>x>>y;
		int a= 0 , b=0;
		if(x%10==0)
		{
			a = x/10;
		}
		else
		{
			a = x/10+1;
		}
		if(y%10==0)
		{
			b = y/10;
		}
		else
		{
			b = y/10+1;
		}
		cout<<"  "<<abs(a-b)<<endl;
	}
}
```