#include <iostream>
using namespace std;
bool isSafe(int** arr,int x,int y,int n){
    for (int row = 0; row < x; row++)
    {
       if (arr[row][y]==1)
       
       return false;
       
       
    }
    int row=x;
    int col=y;
    while(row>=0 && col>=0){
        if(arr[row][col]==1) return false;
        row--;
        col--;
    }
    row=x;
    col=y;
    while(row>=0 && col<n){
        if(arr[row][col]==1) return false;
        row--;
        col++;
    }

return true;
    
}
int nqueen(int** arr,int x,int n){
    if(x>=n) return 1;
    int ans=0;
    for (int col = 0; col < n; col++)
    {
        if (isSafe(arr,x,col,n))
        {
           arr[x][col]=1;
           ans+=nqueen(arr,x+1,n);
           
           }
 arr[x][col]=0;
        
       
    }
    
    return ans;
}
int main(){
    int n;
    cin>>n;
    int** arr=new int*[n] ;
    for (int i = 0; i < n; i++)
    {
      arr[i]=new int[n];
      for (int j = 0; j < n; j++)
      {
       arr[i][j]=0;
      }
      
    }
    cout<<nqueen(arr,0,n);
    return 0;
}
