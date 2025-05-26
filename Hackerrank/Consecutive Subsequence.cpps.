#include <iostream>
#include <vector>
using namespace std;
 
int main() {
    int T;
    cin >> T;
    while (T--) {
        int n, k;
        cin >> n >> k;
        int sum = 0;
        vector<int> cnt(k);
        cnt[0] = 1;
        for (int i = 0; i < n; i++) {
            int tmp;
            cin >> tmp;
            sum += tmp;
            sum %= k;
            cnt[sum]++;
        }
        long long count = 0;
        for (int i = 0; i < k; i++) {
            count += ((long long)cnt[i] * (cnt[i] - 1) / 2);
        } 
        cout << count << endl;
    }
    return 0;
}
