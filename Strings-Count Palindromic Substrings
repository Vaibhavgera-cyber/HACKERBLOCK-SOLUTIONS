#include<iostream>
using namespace std;
bool isPalindrome(string s,int i,int j){
	while(i<j){
		if(s[i]!=s[j]){
			return false;
		}
		i++;
		j--;
	}
	return true;
}
int main() {
	string s;
	cin>>s;
	int n=s.size();
	int count=0;
	for(int i=0;i<n;i++){
		for(int j=i;j<n;j++){
			if(isPalindrome(s,i,j)){
				count++;
			}
		}
	}
	cout<<count;
	return 0;
}
