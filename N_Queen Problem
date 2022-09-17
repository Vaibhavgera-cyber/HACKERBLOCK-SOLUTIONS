#include<bits/stdc++.h>
using namespace std;

 bool isSafe(string** board,int row,int col,int n){
        // horizontal
        for(int i=0;i<n;i++){
            if(board[row][i] == "Q") return false;
        }
        
        // vertical
        for(int i=0;i<n;i++){
            if(board[i][col] == "Q") return false;
        }
        
        // upper right
        int r=row;
        for(int c=col; c>=0 && r>=0;c--,r--){
            if(board[r][c] =="Q") return false;
        }
        
        // upper left
        r=row;
        for(int c=col;c<n && r>=0;c++,r--){
            if(board[r][c] =="Q") return false;
        }
        
        // lower left
        r=row;
        for(int c=col;c>=0 && r<n;c--,r++){
            if(board[r][c] =="Q") return false;
        }
        
        // lower right
        r=row;
        for(int c=col; c<n && r<n; c++,r++){
            if(board[r][c] =="Q") return false;
        }
        
        return true;
        
    }

void helper(string** board,int n,int row,int& count){
	if(row== n){
	
	for(int i=0;i<n;i++){
		for(int j=0;j<n;j++){
			if(board[i][j] =="Q"){
				cout <<"{" << i+1 << "-"<<j+1 << "} ";
			}
			
		}
		
	}
	cout << "  ";
	count++;
		return;


	}

	for(int col=0;col<n;col++){
		if(isSafe(board,row,col,n)){
			board[row][col]="Q";
			// recursion
			helper(board,n,row+1,count);
			// backtracking
			board[row][col]=".";
		}

	}

	return;

}

int main(){
	int n;
	cin >> n;
	int count=0;
	string** board=new string*[n];
        for(int i=0;i<n;i++){
            board[i]=new string[n];
        }
	helper(board,n,0,count);
	cout << endl;
	cout << count ;
}
