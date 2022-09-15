#include<iostream>
#include<cmath>

using namespace std;

void toh(int n, string from, string to , string help){

    if(n==0)
    {
        return; 
    }
    toh(n-1, from , help, to);
    cout<<"Move "<<n<< "th disc from "<<from<<" to "<<to << endl;
    toh(n-1, help, to ,from);
} 

int main(){
    int n;
    cin >> n;
    string from = "T1";
    string to = "T2";
    string help = "T3";
    toh(n,"T1","T2", "T3");
    cout<< pow(2,n)-1;
}
