#include<iostream>
#include<math.h>
using namespace std;
int sizenum(int n){
	int size=0;
	while(n){
		n/=10;
		size++;
	}
	return size;
}	 
int main(){
	int n1; 
	cin>>n1; 
	int size=sizenum(n1);
	int arr[size];
	int b[size]={0};
	int i=0;
	while(n1){
		arr[i]=n1%10;
		n1/=10;
		i++;
	}
	i=0;
	while(i<size){
		b[arr[i]-1]=i+1;
		i++;
	}
	for(int i=0;i<size;i++){ 
		n1+=b[i]*pow(10,i);
	}
	cout<<n1;
	return 0;
}
