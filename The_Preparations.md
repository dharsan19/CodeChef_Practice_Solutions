# The Preparations
## Problem
Chef has an exam which will start exactly MM minutes from now. However, instead of preparing for his exam, Chef started watching Season-11 of Superchef. Season-11 has NN episodes, and the duration of each episode is KK minutes.

Will Chef be able to finish watching Season-11 strictly before the exam starts?

\textbf{Note:}Note: Please read the explanations of the sample test cases carefully.

## Input Format
The first line contains an integer TT denoting the number of test cases. TT test cases then follow.
The first and only line of each test case contains 33 space separated integers MM, NN and KK.
## Output Format
For each test case, output on one line YES if it is possible to finish Season-1 strictly before the exam starts, or NO if it is not possible to do so.

Output is case insensitive, which means that "yes", "Yes", "YEs", "no", "nO" - all such strings will be acceptable.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int m,n,k;
	    cin>>m>>n>>k;
	    if(m>(n*k))
	    {
	        cout<<"YES"<<endl;
	    }
	    else
	    {
	        cout<<"NO"<<endl;
	    }
	}
	return 0;
}
```