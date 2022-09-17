#include <iostream>
#include <bits/stdc++.h>
using namespace std;

void permute(string s,vector<string> &ans,int i,string temp){
    if(s[i]=='\0'){
        ans.push_back(temp);
        return;
    }

    for(int j=i;j<s.length();j++){
        swap(s[i],s[j]);
        temp = s;
        permute(s,ans,i+1,temp);
        temp="";
        swap(s[i],s[j]);
    }
}

int main(){
    string s;
    cin >> s;

    vector<string> ans;
    permute(s,ans,0,"");

    sort(ans.begin(),ans.end());

    for(int i=0;i<ans.size();i++){
        if(s.compare(ans[i])<1){
            if(ans[i]!=s)
                cout << ans[i] <<endl;
        }
    }
}
