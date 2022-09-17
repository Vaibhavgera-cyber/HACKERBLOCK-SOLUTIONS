#include <iostream>
using namespace std;

void multiple(int x, int *ans, int &nd)
{
    int carry = 0;
    for (int i = 0; i < nd; i++)
    {
        int product = (ans[i] * x) + carry;
        ans[i] = product % 10;
        carry = product / 10;
    }

    while (carry > 0)
    {
        ans[nd] = carry % 10;
        carry = carry / 10;
        nd++;
    }
}
int main()
{
    int n;
    cin >> n;
    int ans[20000];
    ans[0] = 1;
    int nd = 1;
    for (int i = 2; i <= n; i++)
    {
        multiple(i, ans, nd);
    }
    for (int i = nd; i >= 0; i--)
    {
        cout << ans[i];
    }
    return 0;
}
