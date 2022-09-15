#include <iostream>

using namespace std;

int main()
{
    int n,m;
    cin>>n>>m;
    int arr[n][m];
    for(int i=0;i<n;i++)
    {
        for(int j=0;j<m;j++)
        {
            cin>>arr[i][j];
        }
    }
    
    int i=0;
    int j=0;
    while(j<m)
    {
        if(j%2==0)
        {
            i=0;
            while(i<n)
            {
                cout<<arr[i][j]<<", ";
                i++;
            }
        }
        else
        {
            i=n-1;
            while(i>=0)
            {
                cout<<arr[i][j]<<", ";
                i--;
            }
        }
        j++;
    }
	cout<<"END";

    return 0;
}
