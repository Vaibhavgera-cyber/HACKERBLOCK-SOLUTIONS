
#include <iostream>
#include<bits/stdc++.h>
using namespace std;

int main()
{
    
    int n;
    cin>>n;
    
    vector<vector<int>>matrix(n,vector<int>(n));
    
    for(int i=0;i<n;i++){
        for(int j=0;j<n;j++){
            cin>>matrix[i][j];
        }
    }
    
    vector<int>v;
    
    for(int i=0;i<n;i++){
        int a=0;
        for(int j=0;j<n;j++){
            if(matrix[i][j]==1){
                a=1;
                break;
            }
        }
        if(a==0)
        v.push_back(i);
    }
    
    for(auto i:v){
        int a=0;
        for(int j=0;j<n;j++){
            if(i==j)continue;
            if(matrix[j][i]==0){
                a=1;
                break;
            }
        }
        
        if(a==0){
            cout<<i<<endl;
            return 0;
        }
    }
    cout<<"No Celebrity"<<endl;

    return 0;
}
