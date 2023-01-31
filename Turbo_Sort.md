# Turbo Sort
## Problem
Given the list of numbers, you are to sort them in non decreasing order.

## Input
t – the number of numbers in list, then t lines follow [t <= 10^6].
Each line contains one integer: N [0 <= N <= 10^6]

## Output
Output given numbers in non decreasing order.

```cpp
#include <bits/stdc++.h>

using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	vector <int> a(t);
	for(int i = 0; i< t ; i++){
	    cin>>a[i];
	}
	sort(a.begin(),a.end());
	for(int i = 0;i<t;i++)
	    cout<<a[i]<<endl;
	return 0;
}
```