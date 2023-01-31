# Score High
## Problem
Chef is taking a tough examination. The question paper consists of N objective problems and each problem has 4 options A,B,C, and D, out of which, exactly one option is correct.

Since Chef did not study for the exam, he does not know the answer to any of the problems. Chef was looking nearby for help when his friend somehow communicated the following information:

Exactly N A problems have option A as the answer.
Exactly N B problems have option B as the answer.
Exactly N C problems have option C as the answer.
Exactly N D problems have option D as the answer.
Note that:
N A+N B+N C+N D=N.
Each problem is worth exactly 1 mark and there is no negative marking.
Even though Chef knows the number of correct options of each type, he does not know the correct answer to any problem.
Based on the given information, find the maximum marks Chef can guarantee if he marks the answers optimally.

## Input Format
First line will contain T, number of test cases. Then the test cases follow.
First line of each test case contains an integer N denoting the number of problems.
Second line of each test case contains 4 integers N A,N B,N C, and N D- as mentioned in the problem statement.
## Output Format
For each test case, output the maximum marks Chef can guarantee if he marks the answers optimally.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n,arr[4];
	    cin>>n;
	    int max = 0;
	    for(int i = 0; i<4; i++)
	    {
	        cin>>arr[i];
	        if(arr[i] > max)
	            max = arr[i];
	    }
	    cout<<max<<endl;
	}
	return 0;
}
```