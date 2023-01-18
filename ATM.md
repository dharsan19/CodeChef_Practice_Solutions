# ATM
## Problem
Pooja would like to withdraw X $US from an ATM. The cash machine will only accept the transaction if X is a multiple of 5, and Pooja's account balance has enough cash to perform the withdrawal transaction (including bank charges). For each successful withdrawal the bank charges 0.50 $US.

Calculate Pooja's account balance after an attempted transaction.

## Input Format
Each input contains 2 integers X and Y.
X is the amount of cash which Pooja wishes to withdraw. Y is Pooja's initial account balance.

## Output Format
Output the account balance after the attempted transaction, given as a number with two digits of precision. If there is not enough money in the account to complete the transaction, output the current bank balance.

```cpp
#include <iostream>
using namespace std;

int main() {
    int w;
    float ac_bl;
    cin>>w;
    cin>>ac_bl;
    if(w%5==0 && w<=ac_bl-0.5){
        cout<<((ac_bl-w)-(0.5));
    }
    else{
        cout<<ac_bl;
    }
	return 0;
}
```