#include <bits/stdc++.h>

using namespace std;

int main() {
    int leftmax, rightmax;
	int t;
	cin>>t;
	while(t--){
	int n;
	cin>>n;
	int height[n];
	for(int i =0 ; i<n; i++){
		cin>>height[i];
	}
    //int height[1000] = {0,2,1,3,0,1,2,1,2,1};
    
    int water=0;
    for(int i = 1; i<n; i++){
        int j = i-1;
        leftmax = 0;
        rightmax = 0;
        
        while(j >= 0){
            leftmax = max(height[j] , leftmax);
            j--;
        }
        int k = i+1;
        while(k < n){
            rightmax = max(height[k], rightmax);
            k++;
        }
        
       // cout<<leftmax << " "<<rightmax << endl;
        int curr = (min(leftmax,rightmax)) - height[i];
        if(curr < 0)
        {
            continue;
        }
        water += curr;
        
    }
    cout<<water<<endl;
	}

}
