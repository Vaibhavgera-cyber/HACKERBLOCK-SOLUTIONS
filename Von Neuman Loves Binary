#include<iostream>
#include <bits/stdc++.h>
using namespace std;
int main() {
	int t;
	cin>>t;
	while(t--){
		int n;
		int bin=0;
		int power=0;
		cin>>n;
		while(n>0){
			if(n%10==1){
				bin+=pow(2,power);
			}
			power++;
			n=n/10;
		}
		cout<<bin<<"\n";
	}

	return 0;
}
