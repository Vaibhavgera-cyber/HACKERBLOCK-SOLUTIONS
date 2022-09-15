#include<iostream>
#include<bits/stdc++.h>
using namespace std;
int main() {
	int n;
	cin>>n;
	int arr[n];
	for(int i=0;i<n;i++){
		cin>>arr[i];
	}
	int min_price=INT_MAX;
	int profit=0;
	for(int i=0;i<n;i++){
		min_price=min(min_price,arr[i]);
		profit=max(profit,arr[i]-min_price);
	}
	cout<<profit;
	return 0;
}
