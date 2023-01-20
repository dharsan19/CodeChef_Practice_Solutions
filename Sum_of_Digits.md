# Sum of Digits
## Problem
You're given an integer N. Write a program to calculate the sum of all the digits of N.

## Input Format
The first line contains an integer T, the total number of testcases. Then follow T lines, each line contains an integer N.

## Output Format
For each test case, calculate the sum of digits of N, and display it in a new line.

```cpp
#include <iostream>
using namespace std;

int main() 
{
    int t;
    cin>>t;
    while(t--)
    {
        int num;
        cin>>num;
        int sum=0;
        while(num)
        {
            sum+=num%10;
            num = num/10;
        }
        cout<<sum<<endl;
    }

	return 0;
}

```