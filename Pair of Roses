#include<iostream>
#include<bits/stdc++.h>
using namespace std;
int main() {
	int t;
	cin>>t;
	while(t--){
		int n;
		cin>>n;
		int arr[n];
		for(int i=0;i<n;i++){
			cin>>arr[i];
		}
		int sum;
		cin>>sum;
		int i=0;
		int j=n-1;
		int r1,r2;
		sort(arr,arr+n);
		while(i<j){
			if(arr[i]+arr[j]==sum){
				r1=arr[i];
				r2=arr[j];
				i++;
				j--;
			}
			else if(arr[i]+arr[j]>sum){
				j--;
			}
			else{
				i++;
			}
		}
		cout<<"Deepak should buy roses whose prices are "<<r1<< " and "<<r2<<".\n";

	}
	return 0;
}
