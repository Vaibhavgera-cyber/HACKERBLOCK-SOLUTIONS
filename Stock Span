

#include <iostream>
#include<bits/stdc++.h>
using namespace std;

int main()
{
    int n;
    cin>>n;
    
    int arr[n];
    
    
    for(int i=0;i<n;i++)cin>>arr[i];
    
//     5
// 30
// 35
// 40
// 38
// 35

vector<int>ans;
    stack<int>s;
    s.push(-1);
    
    for(int i=0;i<n;i++){

        while(!s.empty() && s.top()!=-1 && arr[s.top()]<arr[i]){
            s.pop();
            
        }
        
        ans.push_back(i-s.top());
        s.push(i);
    }

   for(auto i:ans)cout<<i<<" ";
   cout<<"END"<<endl;
    return 0;
}
