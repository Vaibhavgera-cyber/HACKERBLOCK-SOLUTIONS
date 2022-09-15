#include<bits/stdc++.h>
#include<cstring>
#include<string>

using namespace std;

int strToint(string sub){
	
	int num, i=0;
	num = 0;
	while(sub[i]>= '0' && sub[i]<='9'){
		num = num*10 + (sub[i] - '0');
		i++;
	}
	return num;
}

bool isCBnumber(string sub){
	long num = strToint(sub);
	if(num == 0 || num == 1) return false;
	
	int arr[] = {2,3,5,7,11,13,17,19,23,29};
	for(int i = 0; i<10; i++){
		if(num == arr[i]) return true;
		else if(num%arr[i] == 0) return false;		
	}
	return true;
}

bool isvalid( bool *visited , int left , int right){
	for(int i = left; i<right; i++){
		if(visited[i])return false;	
	}
	return true;
}

int main(){

	int n; 
	cin>>n;
	
	string s;
	cin>>s;
	
	int size = s.length();
	
	long count = 0;
	
	bool visited[100];
	
	for(int i =0; i<size; i++){
		visited[i]=false;
	}
	for(int i = 1; i<=size; i++){
		for(int j =0; j<= size-i; j++){
			int e = j+i;
			
			string sub = s.substr(j, e-j);
			if(isCBnumber(sub) && isvalid(visited, j , e)){
				count++;
				for(int k = j; k<e; k++){
					visited[k] = true;
				}
			}
		}
	}
	cout<<count<<endl;
	
	
	
	return 0;
	
}
