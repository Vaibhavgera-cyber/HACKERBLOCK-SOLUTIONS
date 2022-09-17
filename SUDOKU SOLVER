#include <iostream>
#include <vector>
using namespace std;
int N = 9;
bool isSafe(vector<vector<int>> &grid,int row,int col,int num){
    for(int i=0;i<9;i++){ //9
        if(grid[row][i]==num){
            return false;
        }
    }
    for(int i=0;i<9;i++){ //9
        if(grid[i][col]==num){
            return false;
        }
    }
    int currRow = (row/3) * 3; // updated
    int currCol = (col/3) * 3;
    for(int i=0;i<3;i++){
        for(int j=0;j<3;j++){
            if(grid[i+currRow][j+currCol] == num){
                return false;
            }
        }
    }
    return true;
}
bool solveSudoku(vector<vector<int>> &grid,int row,int col){
    if(row==N){
        return true;
    }
    if(col == N){
        return solveSudoku(grid,row+1,0); // updated
    }
    if(grid[row][col] != 0){
        return solveSudoku(grid,row,col+1);
    }
    for(int num = 1;num <=9;num++){
        if(isSafe(grid,row,col,num)){
            grid[row][col] = num;
            if(solveSudoku(grid,row,col+1)){
                return true;
            }
            grid[row][col] = 0;
        }
    }
    return false;
}
int main() {
    // int N=9;
    cin >> N;
    vector<vector<int>> grid;
    for(int i=0;i<N;i++){
        vector<int> tmp;
        for(int j=0;j<N;j++){
            // cin >> grid[i][j];
            int t;
            cin >> t;
            tmp.push_back(t);
        }
        grid.push_back(tmp);
    }
        // int grid[N][N] = { { 3, 0, 6, 5, 0, 8, 4, 0, 0 },
        //                { 5, 2, 0, 0, 0, 0, 0, 0, 0 },
        //                { 0, 8, 7, 0, 0, 0, 0, 3, 1 },
        //                { 0, 0, 3, 0, 1, 0, 0, 8, 0 },
        //                { 9, 0, 0, 8, 6, 3, 0, 0, 5 },
        //                { 0, 5, 0, 0, 9, 0, 6, 0, 0 },
        //                { 1, 3, 0, 0, 0, 0, 2, 5, 0 },
        //                { 0, 0, 0, 0, 0, 0, 0, 7, 4 },
        //                { 0, 0, 5, 2, 0, 6, 3, 0, 0 } };
    if (solveSudoku(grid, 0, 0)){
        for(int i=0;i<N;i++){
            for(int j=0;j<N;j++){
                cout << grid[i][j]<<" ";
            }
            cout << endl;
        }
    }
}
/*
Output
3 1 6 5 7 8 4 9 2
5 2 9 1 3 4 6 7 8
4 8 7 2 6 9 5 3 1
2 6 3 4 1 5 9 8 7
9 7 4 8 6 3 1 2 5
8 5 1 7 9 2 6 4 3
1 3 8 9 4 7 2 5 6
6 9 2 3 5 1 8 7 4
7 4 5 2 8 6 3 1 9
*/
