# Count the Notebooks
## Problem
You know that 1 kg of pulp can be used to make 1000 pages and 1 notebook consists of 100 pages.

Suppose a notebook factory receives N kg of pulp, how many notebooks can be made from that?

## Input Format
First line will contain T, the number of test cases. Then the test cases follow.
Each test case contains a single integer N - the weight of the pulp the factory has (in kgs).
## Output Format
For each test case, output the number of notebooks that can be made using N kgs of pulp.

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
	    cout<<n*10<<endl;
	}
	return 0;
}
```