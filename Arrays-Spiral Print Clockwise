#include<iostream>
using namespace std;
int main(){
    
    int n,m;
    cin>>n>>m;
    int arr[n][m];
    for(int i=0;i<n;i++){
        for(int j=0;j<m;j++){
            cin>>arr[i][j];
        }
    }
    
    int row_start=0,col_start=0,row_end=n-1,col_end=m-1;
    
    while(row_start<=row_end&&col_start<=col_end){
		int j=col_start;
        while(j<=col_end){
            cout<<arr[row_start][j]<<", ";
            j++;
        }
        row_start++;
        
		j=row_start;
        while(j<=row_end){
            cout<<arr[j][col_end]<<", ";
            j++;
        }
        col_end--;
        
		if(row_start<=row_end){ 			
			j=col_end;
			while(j>=col_start){
				cout<<arr[row_end][j]<<", ";
				j--;
			}
		}
        row_end--;
        
		if(col_start<=col_end){
			j=row_end;
			while(j>=row_start){
				cout<<arr[j][col_start]<<", ";
				j--;
			}
		}
		
        col_start++;
        
    }
	cout<<"END";
   
    
    
    
    
    
    return 0;
}
