# Enormous Input Test
## Problem
You are given N integers. Find the count of numbers divisible by K.

## Input Format
The input begins with two positive integers N, K. The next N lines contains one positive integer each denoted by Ai.

## Output Format
Output a single number denoting how many integers are divisible by K.

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,k;
    cin>>n>>k;
    int count = 0;
    while(n--)
    {
        int num;
        cin>>num;
        if(num % k == 0)
        {
            count++;
        }
        
    }
    cout<<count<<endl;
    return 0;
}
```