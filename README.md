# create-palindrome-using-stack

#include<iostream>
#include<string.h>
#include<sstream>
#include<stack>

using namespace std;
int main()
{
	string str;
	getline(cin, str);
	int n = str.length();
	stack<char> s;

	for (int i = 0; i < n; i++)
	{
		s.push(str.at(i));
		cout << str.at(i);
	}
	for (int i = 0; i < n; i++)
	{
		cout << s.top();
		s.pop();
	}		
  return 0;
}
