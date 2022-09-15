#include<iostream>
using namespace std;
bool time_taken(int arr[],int m,int n,int k){
	int timeTaken=0;
	int painters=1;
	for(int i=0;i<n;i++){
		if(timeTaken+arr[i]<=m){
			timeTaken+=arr[i];
		}
		else{
			painters++;
			if(painters>k || arr[i]>m){ 
				return false;
			}
			timeTaken=arr[i];
		}
	}
	return true;

}
int main() {
	int k;
	cin>>k;
	int n;
	cin>>n;
	int arr[n];
	int sum=0;
	for(int i=0;i<n;i++){
		cin>>arr[i];
		sum+=arr[i];
	}
	int s=0,e=sum;
	int m=s+(e-s)/2;
	int ans=0;
	while(s<=e){
		if(time_taken(arr,m,n,k)){ 
			ans=m;
			e=m-1;
		}
		else{
			s=m+1;
		}
		m=s+(e-s)/2;
	}
	cout<<ans;
	return 0;
}
