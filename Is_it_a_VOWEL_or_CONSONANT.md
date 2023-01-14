# Is it a VOWEL or CONSONANT
## Problem
Write a program to take a character (C)(C) as input and check whether the given character is a vowel or a consonant.

NOTE:-NOTE:− Vowels are 'A', 'E', 'I', 'O', 'U'. Rest all alphabets are called consonants.

## Input Format
First line will contain the character CC.
Output Format
Print "Vowel" if the given character is a vowel, otherwise print "Consonant".

## Constraints
CC willwill bebe anan upperupper casecase EnglishEnglish alphabetalphabet
```cpp
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	char c;
	cin>>c;
	
	bool is_vowel;
	is_vowel = ( c == 'A' || c == 'E' || c == 'I' || c == 'O' || c == 'U');
	
	if(is_vowel)
	{
	    cout<<"Vowel"<<endl;
	}
	else
	{
	    cout<<"Consonant"<<endl;
	}
	return 0;
}

```