### Hi there 👋

<!--
**CatIsa1/catisa1** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

#include <iostream>
#include <cstring>

using namespace std;

bool isPalindrome(string str) {
    int n = str.length();
    for (int i = 0; i < n/2; i++) {
        if (str[i] != str[n-i-1]) {
            return false;
        }
    }
    return true;
}

int main() {
    string str;
    cout << "Enter a string: ";
    cin >> str;

    if (isPalindrome(str)) {
        cout << str << " is a palindrome." << endl;
    } else {
        cout << str << " is not a palindrome." << endl;
    }
    return 0;
}
