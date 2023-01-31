# Finding Square Roots
## Problem 

In olden days finding square roots seemed to be difficult but nowadays it can be easily done using in-built functions available across many languages .

Assume that you happen to hear the above words and you want to give a try in finding the square root of any given integer using in-built functions. So here's your chance.

## Input
The first line of the input contains an integer T, the number of test cases. T lines follow. Each line contains an integer N whose square root needs to be computed.

## Output
For each line of the input, output the square root of the input integer, rounded down to the nearest integer, in a new line.

```cpp
#include <iostream>
#include <math.h>
using namespace std;
int main()
{
   int t;
   cin >> t;
//   if (t >= 1 && t <= 20)
//   {
      while (t--)
      {
         int n;
         cin >> n;
        //  if(n>=1 && n<=10000)
        //  {
            cout << int(sqrt(n)) << endl;
        //  }
         
      }
//   }

   return 0;
}

```