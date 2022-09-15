#include<bits/stdc++.h>
using namespace std;
int main() {
	int n;
	cin>>n;
	int arr[n];
	for(int i=0;i<n;i++){
		cin>>arr[i];

	}
	int q;
	cin>>q;
	while(q--){
		int amount,k;
		cin>>amount>>k;
		int cnt =0;
		for(int i=0;i<n;i++){
			if(amount % arr[i]==0){
				cnt++;
			}
		}
		if(cnt>=k){
			cout<<"Yes"<<endl;
		}
		else{
			cout<<"No"<<endl;
		}
	}
	return 0;
}
