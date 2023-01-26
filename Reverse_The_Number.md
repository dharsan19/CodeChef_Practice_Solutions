# Reverse The Number
## Problem
Given an Integer N, write a program to reverse it.

## Input
The first line contains an integer T, total number of testcases. Then follow T lines, each line contains an integer N.

## Output
For each test case, display the reverse of the given number N, in a new line.

```cpp
#include <iostream>
using namespace std;

int main() {
    int t;
    cin>>t;
    while(t--)
    {
        int num;
        cin>>num;
        int reverse = 0;
        for(;num>0; num = num/10)
        {
            reverse = reverse*10 + num%10;
        }
        cout<<reverse<<endl;
    }
	return 0;
}
```