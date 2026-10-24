# task-5
#include <iostream>

using namespace std;

int main() {
    int n;
    cin >> n;

    for (int i = 1; i <= n; ++i) {
        for (int j = 0; j < i; ++j) {
            cout << '*';
        }
        cout << endl;
    }

    long long temp = n;
    int kroky = 0;
    while (temp > 1) {
        if (temp % 2 == 0) {
            temp /= 2;
        } else {
            temp = 3 * temp + 1;
        }
        kroky++;
    }

    cout << "kroky: " << kroky << endl;

    return 0;
}
