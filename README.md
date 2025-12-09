#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false);
    cin.tie(nullptr);

    int t;
    cin >> t;

    while(t--) {
        int n, m;
        cin >> n >> m;

        vector<int> c(n);
        for(int i = 0; i < n; i++) cin >> c[i];

        vector<int> mask(m);
        for(int i = 0; i < m; i++) cin >> mask[i];

    
        int needOdd = 0;
        for(int i = 0; i < m; i++) {
            if(mask[i] == 1) needOdd++;
        }

      
        if(needOdd % 2 == 1) {
            cout << 0 << "\n";
        } else {
           
            cout << 1 << "\n";
        }
    }

    return 0;
}
