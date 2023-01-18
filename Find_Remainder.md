# Find Remainder
## Problem
Write a program to find the remainder when an integer A is divided by an integer B.

## Input
The first line contains an integer T, the total number of test cases. Then T lines follow, each line contains two Integers A and B.

## Output
For each test case, find the remainder when A is divided by B, and display it in a new line.

```cpp
#include<iostream>
using namespace std;
int main(){
     int t;
     cin>>t;
     while(t--){
          int a,b,c,d;
          cin>>a>>b;
          if (a>=b){
               c=a%b;
               cout<<"\n"<<c;
          }
          else
          {d=a%b;
          cout<<"\n"<<d;}
     }
     return 0;
}
```