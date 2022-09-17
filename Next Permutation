#include<bits/stdc++.h>
using namespace std;


class solution{
public:

vector<int> nextPermutation(int N, vector<int> arr){
        
        next_permutation(arr.begin(), arr.end());
        return arr; 
    }
};


int main() {

	int t;
	cin >> t;

	while(t--){

		int n; 
		cin >> n;

		vector<int> arr(n);

		for(int i =0; i< n; i++){
			cin>>arr[i];
		}
		solution ob;
		vector<int> ans = ob.nextPermutation(n, arr);
        for(int u: ans)
            cout<<u<<" ";
		cout<<"\n";

	}

	return 0;
}
