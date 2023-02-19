# Mileage matters
## Problem
Chef wants to rent a car to travel to his restaurant which is N kilometers away. He can either rent a petrol car or a diesel car.

One litre of petrol costs X rupees and one litre of diesel costs Y rupees. Chef can travel A kilometers with one litre of petrol and B kilometers with one litre of diesel.

Chef can buy petrol and diesel in any amount, not necessarily integer. For example, if X=95, Chef can buy half a litre of petrol by paying 95/2=47.5 rupees.

Which car should the chef rent in order to minimize the cost of his travel?

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
The first and only line of each test case contains 5 space-separated integers, N,X,Y,A, and B - distance that chef needs to travel, the per litre prices of petrol and diesel and the distance chef can travel using one litre of petrol and diesel respectively.
## Output Format
For each test case, output on a new line PETROL if the cost of travel is less using petrol car, DIESEL if the cost of travel is less using diesel car or ANY if cost of travel is same in both the cases.

You may print each character of the string in either uppercase or lowercase (for example, the strings PETrol, petrol, Petrol,  and PETROL will all be treated as identical). 

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    float n,x,y,a,b;
	    cin>>n>>x>>y>>a>>b;
	    if(((n/a)*x) > ((n/b)*y))
	        cout<<"DIESEL"<<endl;
	    else if(((n/a)*x) == ((n/b)*y))
	        cout<<"ANY"<<endl;
	    else
	        cout<<"PETROL"<<endl;
	    
	}
	return 0;
}
```