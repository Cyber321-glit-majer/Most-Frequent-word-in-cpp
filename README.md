# Most-Frequent-word-in-cpp

**PROBLE STATEMENT**



The following letters of the English alphabet are vowols: a, e,i,o,u. You are given a string named str of length n 
find and print the most frequent vowel in str.

**INPUT**
1. First line containg length of string
2. 2.second line contain string

**OUTPUT**
Most frequent vowel letter in string

```


#include<bits/stdc++.h>
using namespace std;
int main()
{
    int n;
    cin>>n;
    string s;
    cin>>s;
    unordered_map<char,int>mp;
     for(int i=0;i<n;i++)
     {
         if(s[i]=='a' || s[i]=='i' || s[i]=='o'|| s[i]=='u'|| s[i]=='e')
         mp[s[i]]++;
     }
    int currentMax = 0;
int checked = 0;
char maax;
for(auto it = mp.cbegin(); it != mp.cend(); ++it )
    //checked = it->second;
    if (it ->second > currentMax)
    {
        maax = it->first;
    }
    //if(it ->second > currentMax){
    //v = it->first
    cout<<maax;
}
