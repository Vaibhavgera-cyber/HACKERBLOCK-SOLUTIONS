#include<bits/stdc++.h>
using namespace std;
bool compare(int arr[],int n,int c,int mid){
	int count=1;
	int cow=arr[0];
	for(int i=0;i<n;i++){
		if(arr[i]-cow>=mid){
			
			cow=arr[i];
			count++;
			if(count==c){
				return true;
			}
		}
	}
	if(count<c){
		return false;
	}
	return true;
}
int main(){
	int n,c,ans;
	cin>>n>>c;
	int arr[n];
	for(int i=0;i<n;i++){
		cin>>arr[i];
	}
	sort(arr,arr+n);
	int start=0;
	int end=n-1;
	ans=0;
	while(start<=end){
int mid=start+(end-start)/2;
bool hello=compare(arr,n,c,mid);
if(hello){
	ans=mid;
	start=mid+1;
}
else{
	end=mid-1;
}


	}
cout<<ans<<endl;
return 0;
}
