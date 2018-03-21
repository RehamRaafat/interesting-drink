#include <bits/stdc++.h>

using namespace std;

int main()
{
    int n,x;
    vector<int>v;
    cin>>n;
    for(int i=0; i<n; i++)
    {
        int y;
        cin>>y;
        v.push_back(y);
    }
    sort(v.begin(),v.end());
    cin>>x;
    for(int j=0; j<x; j++)
    {
       int a;
       cin>>a;
       cout<<upper_bound(v.begin(),v.end(),a)-v.begin()<<endl;
    }
    return 0;
}
