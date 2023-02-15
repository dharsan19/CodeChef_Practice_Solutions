# Degree of Polynomial
## Problem
In mathematics, the degree of polynomials in one variable is the highest power of the variable in the algebraic expression with non-zero coefficient.

Chef has a polynomial in one variable x with N terms. The polynomial looks like A 0 ⋅x 0 +A 1 ⋅x 1 +…+A N−2 ⋅x N−2 +A N−1 ⋅x N−1  where A i−1  denotes the coefficient of the i th  term x i−1  for all (1≤i≤N).

Find the degree of the polynomial.

Note: It is guaranteed that there exists at least one term with non-zero coefficient.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
First line of each test case contains of a single integer N - the number of terms in the polynomial.
Second line of each test case contains of N space-separated integers - the i th  integer A i−1  corresponds to the coefficient of x i−1 .
## Output Format
For each test case, output in a single line, the degree of the polynomial.

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
	    int arr[n],count = 0;
	    for(int i = 0; i<n; i++)
	    {
	        cin>>arr[i];
	    }
	    if(n == 1)
	    {
	        cout<<0<<endl;
	    }
	    else
	    {
	       count = n-1;
	       while(n--)
	       {
	           if(arr[n] == 0)
	           {
	               count--;
	           }
	           else
	           {
	               break;
	           }
	       }
	       cout<<count<<endl;
	    }
	}
	return 0;
}
```