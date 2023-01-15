# Email Reminders
## Problem
MoEngage helps the Chef send email reminders about rated contests to the participants.

There are a total of NN participants on Chef’s platform, and UU of them have told Chef not to send emails to them.

If so, how many participants should MoEngage send the contest emails to?

## Input Format
The first and only line of input will contain a single line containing two space-separated integers NN (the total number of users) and UU (the number of users who don't want to receive contest reminders).
## Output Format
Output in a single line, the number of users MoEngage has to send an email to.
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int n,u;
	cin>>n>>u;
	cout<<n-u<<endl;
	return 0;
}

```