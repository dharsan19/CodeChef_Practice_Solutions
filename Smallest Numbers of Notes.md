# Smallest Numbers of Notes
## Problem
Consider a currency system in which there are notes of six denominations, namely, Rs. 1, Rs. 2, Rs. 5, Rs. 10, Rs. 50, Rs. 100.
If the sum of Rs. N is input, write a program to computer smallest number of notes that will combine to give Rs. N.

## Input
The first line contains an integer T, total number of testcases. Then follow T lines, each line contains an integer N.

## Output
For each test case, display the smallest number of notes that will combine to give N, in a new line.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
        int n;
        cin>>n;
        int a = n%100;
        int b = a%50;
        int c = b%10;
        int d = c%5;
        int e = d%2;
        cout<<(n/100)+(a/50)+(b/10)+(c/5)+(d/2)+e<<endl;
	}
	return 0;
}
```