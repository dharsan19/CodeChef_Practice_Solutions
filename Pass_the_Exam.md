# Pass the Exam
## Problem
Chef appeared for an exam consisting of 3 sections. Each section is worth 100 marks.
Chef scored A marks in Section 1, B marks in section 2, and C marks in section 3.
Chef passes the exam if both of the following conditions satisfy:
Total score of Chef is ≥100;
Score of each section ≥10.
Determine whether Chef passes the exam or not.

## Input Format
The first line of input will contain a single integer T, denoting the number of test cases.
Each test case consists of a single line containing 3 space-separated numbers A,B,C - Chef's score in each of the sections.
## Output Format
For each test case, output PASS if Chef passes the exam, FAIL otherwise.

Note that the output is case-insensitive i.e. PASS, Pass, pAsS, and pass are all considered same.

```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b,c;
	    cin>>a>>b>>c;
	    int total;
	    total = a+b+c;
	    if(total>=100 && a>=10 && b>=10 && c>=10)
	    {
	        cout<<"PASS"<<endl;
	    }
	    else
	    {
	        cout<<"FAIL"<<endl;
	    }
	}
	return 0;
}
```